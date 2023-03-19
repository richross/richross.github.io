---
layout: posts
title: Another Reason to Use Devcontainers!
author: Rich Ross
excerpt_separator: <!--more-->
---

I've been a huge fan [Devcontainers](https://containers.dev/) specification.  There are so many use cases and examples of how this definition and the applications that support implemnenting this capability provides for a better development experience and increases 'developer velocity'.  I even use this technology for writing this blog.
<!--more-->

My latest use case is around an open source project called ['Synthea'](https://synthetichealth.github.io/synthea/).  If you've not heard of this, it is a tool for creating patient record data strictly for demo purposes.  The platform is configurable so you can define the population for your demo situation.  In my case, I just need records to populate into a Microsoft Cloud for Healthcare instance as the visits have gotten a little old since building it out a few years ago.

The application is written in java and uses gradle.  Not a problem, but also not something I have installed on my development machine.  Devcontainers was in my plans from the start.

My biggest challenge stems from not noticing the [UNIX notice in the files](/assets/20230310-unix.jpg).  

I cloned the repo onto my Windows machine with the plan to open it in VS Code, use the Remote Development extension to create and load the project into the developer container.  This worked well, but when I went to run the commands for Synthea, I got this error:
``` 
/usr/bin/env: ‘sh\r’: No such file or directory
```
This was a little strange as it mostly matches the 1st line of code in the gradlew file I ran first.  In hindsight, this is also strange as the directory separator is '\' instead of this '/' in my linux conotainer.

As you probably guessed, opening the project on windows added the carriage return ('\r') characters in all of the files in the project.  I can't see them in the file but when the code runs, they are there and linux/unix does not use this code.  With no easy way to remove them, I deleted everything in my repo except the files added when creating the Remote Development container (devcontainer folder and devcontainer.json).  I committed the changes and then did a rebase to pull the unaltered files from my GitHub repo into the local repo.  All of this was done inside my devcontainer and a linux environment.

The additional characters were not added to the files this time and running commands works as expected.  Off to go and create some interesting patient data for experiences.
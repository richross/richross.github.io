---
layout: posts
title: Custom Code Connector Project
author: Rich Ross
excerpt_separator: <!--more-->
---
## {{page.title}}
Microsoft Power Platform represents the power of 'low-code' solution development for the business or citizen developer.  The Custom Connector feature is one of the areas in the platform where pro-developers may initially provide their skills and experience to enable access to line of business (LOB) data in the Power Platform.  The process of creating a Custom Connector is listed in the documentation [here](https://docs.microsoft.com/en-us/connectors/custom-connectors/define-blank).
<!--more-->
The custom connector provides configuration steps to call an API endpoint, provide any required security and make that data available to a PowerApp or Power Automate. A recent enhancement to the original custom connector now provides the ability to manipulate the reponse from the underlying API via a custom C# code class prior to sending the response back to the calling application.  This class needs to inherit from ScriptBase and implement the appropriate interfaces.

The UI for this functionality provvides for uploading a single .cs file.  The interactive textbox does provide for some limited editing.  This means you should have a working file before uploading as the debugging process/feedback is kind of limited.  This [file](https://docs.microsoft.com/en-us/connectors/custom-connectors/write-code) provides information on writing the code section of the custom connector.

Console project for creating 'Code' section of a custom connector.  Includes appropriately named classes and interfaces so all you need to do is upload the Script.cs file.
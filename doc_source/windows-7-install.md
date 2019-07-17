# Amazon Corretto 11 Installation Instructions for Windows 7 or Later<a name="windows-7-install"></a>

 This topic describes how to install and uninstall Amazon Corretto 11 on a host or container running the Windows 7 or later operating system\. 

## Install Amazon Corretto 11<a name="windows-7-install-instruct"></a>

1.  Download a Windows `.msi` file from the [Downloads](downloads-list.md) page\. 

1.  Double\-click the \.msi file to start the installation wizard\. 

1.  Follow the steps in the wizard\. 

    You have the option of setting a custom installation path\. By default, Amazon Corretto 11 is installed at `C:\Program Files\Amazon Corretto\`\. If you set a custom path, make a note of it for the next step\. 

1.  Once the install wizard is finished, set the `JAVA_HOME` and `PATH` environment variables\. 

   Set `JAVA_HOME` to the installation location, noting that the directory contains the currently\-installed version\. For example, if the default directory is used for 11\.0\.4, then set `JAVA_HOME` as `C:\Program Files\Amazon Corretto\jdk11.0.4_11`\.

   Add `%JAVA_HOME%\bin` to the current `PATH` variable\.

1.  Verify the installation by running java \-version in a command prompt\. You should see the following output\.   
**Example**  

   ```
   openjdk version "11.0.4" 2019-07-16 LTS
   OpenJDK Runtime Environment Corretto-11.0.4.11.1 (build 11.0.4+11-LTS)
   OpenJDK 64-Bit Server VM Corretto-11.0.4.11.1 (build 11.0.4+11-LTS, mixed mode)
   ```

## Uninstall Amazon Corretto 11<a name="windows-7-uninstall"></a>

You can uninstall Amazon Corretto 11 by following the standard steps to uninstall an application from Windows\.

1.  Open **Programs and Features**\. 

1.  Search for **Amazon Corretto 11** and then select it\. 

1.  Choose **uninstall**\. 
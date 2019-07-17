# Amazon Corretto 11 Installation Instructions for Debian\-Based and RPM\-Based Linux Distributions<a name="generic-linux-install"></a>

This topic describes how to install Amazon Corretto 11 on Debian\-based and RPM\-based Linux distributions\. 

## Install Amazon Corretto 11 on Debian\-Based Linux<a name="debian-install-instruct"></a>

This section describes how to install and uninstall Amazon Corretto 11 on a host or container running a Debian\-based operating system\.

### Download and Install the Debian Package Manually<a name="debian-deb-install-instruct"></a>

1.  Before you install the JDK, install the `java-common` package\.   
**Example**  

   ```
   sudo apt-get update && sudo apt-get install java-common
   ```

1.  Download the Linux `.deb` file from the [Downloads](downloads-list.md) page\. 

1.  Install the `.deb` file by using `sudo dpkg --install`\.   
**Example**  

   ```
   sudo dpkg --install 
   ```

### Verify Your Installation<a name="debian-deb-verify"></a>

 In the terminal, run the following command to verify the installation\. 

**Example**  

```
java -version
```
Expected output for 11\.0\.4:   

```
openjdk version "11.0.4" 2019-07-16 LTS
OpenJDK Runtime Environment Corretto-11.0.4.11.1 (build 11.0.4+11-LTS)
OpenJDK 64-Bit Server VM Corretto-11.0.4.11.1 (build 11.0.4+11-LTS, mixed mode)
```

 If you see a version string that doesn't mention `Corretto`, run the following command to change the default `java` or `javac` providers\. 

**Example**  

```
sudo update-alternatives --config java
```
If you're using the JDK, you should also run the following\.  

```
sudo update-alternatives --config javac
```

### Uninstall Amazon Corretto 11<a name="debian-deb-uninstall"></a>

You can uninstall Amazon Corretto 11 by using the following command\.

**Example**  

```
sudo dpkg --remove java-11-amazon-corretto-jdk
```

## Install Amazon Corretto 11 on RPM\-Based Linux<a name="rpm-linux-install-instruct"></a>

### Download and install RPM package manually<a name="rpm-install-instruct"></a>

1.  Download the Linux `.rpm` file from the [Downloads](downloads-list.md) page\. 

1.  Install the downloaded `.rpm` file using `yum localinstall`\.   
**Example**  

   ```
   sudo yum localinstall 
   ```

### Verify Your Installation<a name="rpm-verify"></a>

 In the terminal, run the following command to verify the installation\. 

**Example**  

```
java -version
```
This is the expected output for 11\.0\.4:   

```
openjdk version "11.0.4" 2019-07-16 LTS
OpenJDK Runtime Environment Corretto-11.0.4.11.1 (build 11.0.4+11-LTS)
OpenJDK 64-Bit Server VM Corretto-11.0.4.11.1 (build 11.0.4+11-LTS, mixed mode)
```

 If you see a version string that doesn't mention `Corretto`, run the following command to change the default `java` or `javac` providers\. 

**Example**  

```
sudo alternatives --config java
```
If you're using the JDK, you should also run the following\.  

```
sudo alternatives --config javac
```

### Uninstall Amazon Corretto 11<a name="rpm-uninstall"></a>

You can uninstall Amazon Corretto 11 by using the following

**Example**  

```
sudo yum remove java-11-amazon-corretto-devel
```
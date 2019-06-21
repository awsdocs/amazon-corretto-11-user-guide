# Amazon Corretto 11 Installation Instructions for Amazon Linux 2<a name="amazon-linux-install"></a>

 This topic describes how to install and uninstall Amazon Corretto 11 on a host or container running the Amazon Linux 2 operating system\. 

## Install using the yum Package Manager on Amazon Linux<a name="amazon-linux-install-instruct"></a>

 Amazon Corretto 11 has a 'headless' variant available\. This variant omits runtime dependencies that are typically associated with GUI applications such as X11 and ALSA and is worth considering for server\-oriented workloads\. 

Option 1: Install headless Amazon Corretto 11:

**Example**  

```
sudo yum install java-11-amazon-corretto-headless
```

Option 2: Install the full Amazon Corretto 11:

**Example**  

```
sudo yum install java-11-amazon-corretto
```

 The installation location is `/usr/lib/jvm/java-11-amazon-corretto.<cpu_arch>`\. 

## Verify Your Installation<a name="amazon-linux-verify"></a>

 To verify the installation, run `java -version` in a console\. If the version string doesn't mention `Corretto`, run the following command to change the default `java` provider\. 

**Example**  

```
sudo alternatives --config java
```

## Uninstall Amazon Corretto 11<a name="amazon-linux-uninstall"></a>

You can uninstall Amazon Corretto 11 with the following commands\.

Uninstall headless:

**Example**  

```
sudo yum remove java-11-amazon-corretto-headless
```

Uninstall full:

**Example**  

```
sudo yum remove java-11-amazon-corretto
```
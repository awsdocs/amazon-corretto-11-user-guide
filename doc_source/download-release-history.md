# Release History for Amazon Corretto 11<a name="download-release-history"></a>

This topic lists all the downloads available for Amazon Corretto 11\. Choose the appropriate link for your environment's platform:

For the latest version, see [Downloads for Amazon Corretto 11](downloads-list.md)\.

## version\.11\.0\.2\.9\.3 released 2019\-03\-19<a name="11.0.2.9.3"></a>

[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/corretto/latest/corretto-11-ug/download-release-history.html)

**Signature Verification**

Public keys are available and are specific to each release: [11\.0\.2\.9\.3 \(Linux, Windows\)](https://d3pxv6yz143wms.cloudfront.net/11.0.3.7.1/11E0D862.pub) and [11\.0\.2\.9\.3 \(macOS\)](gpg.pubkey.url.11.0.2.9.3-1;)\. 

In the terminal, run the following command to verify the installation\.

**Example**  

```
java -version
```
This is the expected output for 11\.0\.2:   

```
openjdk version "11.0.2" 2019-01-15 LTS
OpenJDK Runtime Environment Corretto-11.0.2.9.3 (build 11.0.2+9-LTS)
OpenJDK 64-Bit Server VM Corretto-11.0.2.9.3 (build 11.0.2+9-LTS, mixed mode)
```

 If you see a version string that doesn't mention `Corretto`, run the following command to change the default `java` or `javac` providers\. 
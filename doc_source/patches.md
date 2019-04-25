# List of Patches for Amazon Corretto 11<a name="patches"></a>

This section lists all the patches applied to OpenJDK for Amazon Corretto 11\. We also provide links to the issues in the OpenJDK project\.

**Back port from OpenJDK 12, fixing [JDK\-8202353](https://bugs.openjdk.java.net/browse/JDK-8202353): "os::readdir should use readdir instead of readdir\_r"\.**  
 Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\. Additionally, this also fixes [JDK\-8202835](https://bugs.openjdk.java.net/browse/JDK-8202835): "jfr/event/os/TestSystemProcess\.java fails on missing events"\. 

**Back port from OpenJDK 12, fixing [JDK\-8202794](https://bugs.openjdk.java.net/browse/JDK-8202794): "Native Unix code should use readdir rather than readdir\_r"\.**  
 Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\.

**Back port from OpenJDK 12, fixing [JDK\-8207340](https://bugs.openjdk.java.net/browse/JDK-8207340): "UnixNativeDispatcher close and readdir usages should be fixed"\.**  
 Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\.

**Back port from OpenJDK 12, fixing [JDK\-8207748](https://bugs.openjdk.java.net/browse/JDK-8207748): "Fix for 8202794 breaks tier1 builds"\.**  
 Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\.

**Updates to vendor\-related metadata\.**  
Identifies Amazon as the vendor of this OpenJDK distribution and adds hyperlinks for reporting issues\.
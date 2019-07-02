# Change Log for Amazon Corretto 11<a name="change-log"></a>

The following sections describe the changes for each release of Amazon Corretto 11\.

## Corretto aarch64 preview: version 11\.0\.3\.7\.1<a name="changes-2019-06-28"></a>

Release Date: June 28, 2019

 The following platforms are updated in this release\. 

**Target Platforms**
+  RPM\-based Linux using glibc 2\.17 or later, aarch64 
+  Debian\-based Linux using glibc 2\.17 or later, aarch64 

The following issues and enhancements are addressed in 11\.0\.3\.7\.1\.


| Issue Name | Platform | Description | Link | 
| --- | --- | --- | --- | 
|  Corretto 11 aarch64 preview  |  aarch64  |  add Corretto 11 builds for aarch64\.  |   | 

## April 2019 critical patch update: Corretto version 11\.0\.3\.7\.1<a name="changes-2019-04-16"></a>

Release Date: Apr 16, 2019

 The following platforms are updated in this release\. 

**Target Platforms**
+  RPM\-based Linux using glibc 2\.12 or later, x86\_64 
+  Debian\-based Linux using glibc 2\.12 or later, x86\_64 
+  Windows 7 or later, x86\_64 
+  macOS 10\.13 and later, x86\_64 

The following issues and enhancements are addressed in 11\.0\.3\.7\.1\.


| Issue Name | Platform | Description | Link | 
| --- | --- | --- | --- | 
|  Update Corretto to 11\.0\.3\.7\.1\.  |  All  |  Update Corretto 11 patch set to 11\.0\.3\.7\.1\.  |   | 

## 11\.0\.2\.9\.3: Amazon Corretto 11<a name="changes-2019-03-19"></a>

Release Date: Mar 19, 2019

 The following platforms are updated in this release\. 

**Target Platforms**
+  macOS 10\.13 and later, x86\_64 

The following issues and enhancements are addressed in 11\.0\.2\.9\.3\.


| Issue Name | Platform | Description | Link | 
| --- | --- | --- | --- | 
|  MacOS package installer shows as Corretto 8 instead of Corretto 11\.  |  macOS  |  The message in the introduction session of the mac installer is incorrect\.  |  [corretto\-11\#10](https://github.com/corretto/corretto-11/issues/10)  | 
|  MacOS package installer unable to detect Corretto as a JDK package after installation\.  |  macOS  |  After installing Corretto\-11\.0\.2\.3, /usr/libexec/java\_home is unable to detect it as a JDK package\.  |  [corretto\-11\#12](https://github.com/corretto/corretto-11/issues/12)  | 

## GA release: 11\.0\.2\.9\.3: Amazon Corretto 11<a name="changes-2019-03-14"></a>

Release Date: Mar 14, 2019

 The following platforms are updated in this release\. 

**Target Platforms**
+  RPM\-based Linux using glibc 2\.12 or later, x86\_64 
+  Debian\-based Linux using glibc 2\.12 or later, x86\_64 
+  Windows 7 or later, x86\_64 
+  macOS 10\.13 and later, x86\_64 

The following issues and enhancements are addressed in 11\.0\.2\.9\.3\.


| Issue Name | Platform | Description | Link | 
| --- | --- | --- | --- | 
|  Bump up version string to 11\.0\.2\.9\.3 for GA release\.  |  All  |  Corretto 11 GA release\.  |   | 

## 11\.0\.2\.9\.2: Amazon Corretto 11<a name="changes-2019-03-04"></a>

Release Date: Mar 4, 2019

 The following platforms are updated in this release\. 

**Target Platforms**
+  RPM\-based Linux using glibc 2\.12 or later, x86\_64 
+  Debian\-based Linux using glibc 2\.12 or later, x86\_64 

Added LTS as version\-opt to the version string\.

The following issues and enhancements are addressed in 11\.0\.2\.9\.2\.


| Issue Name | Platform | Description | Link | 
| --- | --- | --- | --- | 
|  Added LTS as version\-opt to the version string\.  |  RPM\-based Linux，Debian\-based Linux  |  Include LTS in the Java version string\.  |   | 

## Initial release: Version Corretto\-11\.0\.2\.9\.1<a name="changes-2019-02-12"></a>

Release Date: Feb 12, 2019

 The following platforms are compatible with this release\. 

**Target Platforms**
+  RPM\-based Linux using glibc 2\.12 or later, x86\_64 
+  Debian\-based Linux using glibc 2\.12 or later, x86\_64 
+  Windows 7 or later, x86\_64 
+  macOS 10\.13 and later, x86\_64 

 The following are the changes for this release\. 


| Patch | Description | Release Date | 
| --- | --- | --- | 
|   Back port from OpenJDK 12, fixing JDK\-8202353: "os::readdir should use readdir instead of readdir\_r"\.   |   Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\. Additionally, this also fixes JDK\-8202835: "jfr/event/os/TestSystemProcess\.java fails on missing events"\.   |   2019\-02\-12   | 
|   Back port from OpenJDK 12, fixing JDK\-8202794: "Native Unix code should use readdir rather than readdir\_r"\.   |   Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\.   |   2019\-02\-12   | 
|   Back port from OpenJDK 12, fixing JDK\-8207340: "UnixNativeDispatcher close and readdir usages should be fixed"\.   |   Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\.   |   2019\-02\-12   | 
|   Back port from OpenJDK 12, fixing JDK\-8207748: "Fix for 8202794 breaks tier1 builds"\.   |   Enables compilation on Amazon Linux 2, as readdir\_r has been deprecated in glibc >= 2\.24\.   |   2019\-02\-12   | 
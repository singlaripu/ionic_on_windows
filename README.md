ionic setup process on windows
================

Download and install the following 

```bash
NodeJS (msi file) - http://nodejs.org/download/
Java SDK jdk-8u5-windows-i586.exe - http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
Github GUI - https://windows.github.com/
Github Commandline - http://git-scm.com/download/win
```

Download the extract below zip files to some folder - I used 'C:\Users\ripu\Desktop\ionic_setup'

```bash
Apache Ant - http://ant.apache.org/bindownload.cgi
Android ADT bundle - http://developer.android.com/sdk/index.html#download
Console2 - http://sourceforge.net/projects/console/
```

Create following new environment variables, change paths as per your system wherever applicable

```bash
ANDROID_HOME : C:\Users\ripu\Desktop\ionic_setup\adt-bundle-windows-x86-20140321\sdk
JAVA_HOME : C:\Program Files\Java\jdk1.7.0_51
```

Edit Enverionment variable "PATH" and add the following (separated by semicolon) - change wherever applicable

```bash
C:\Users\ripu\AppData\Roaming\npm;
C:\Program Files\Java\jdk1.7.0_51\bin;
C:\Users\ripu\Desktop\ionic_setup\apache-ant-1.9.4\bin;
C:\Users\ripu\Desktop\ionic_setup\adt-bundle-windows-x86-20140321\sdk\tools;
C:\Users\ripu\Desktop\ionic_setup\adt-bundle-windows-x86-20140321\sdk\platform-tools;
C:\Program Files\Git\bin
```

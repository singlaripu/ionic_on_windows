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

Please note your jdk version might be different than mine.

Edit Enverionment variable "PATH" and add the following (separated by semicolon) - change wherever applicable

```bash
C:\Users\ripu\AppData\Roaming\npm;
C:\Program Files\Java\jdk1.7.0_51\bin;
C:\Users\ripu\Desktop\ionic_setup\apache-ant-1.9.4\bin;
C:\Users\ripu\Desktop\ionic_setup\adt-bundle-windows-x86-20140321\sdk\tools;
C:\Users\ripu\Desktop\ionic_setup\adt-bundle-windows-x86-20140321\sdk\platform-tools;
C:\Program Files\Git\bin
```

Now double click Console.exe - in my case its located at 'C:\Users\ripu\Desktop\ionic_setup\Console2' and run the following commands

```bash
npm install -g cordova
npm install -g ionic
```

At this point ionic is installed and we are ready to start a project. Navigate to some working directory, I used ionic_setup directory itself.

```bash
cd C:\Users\ripu\Desktop\ionic_setup
ionic start rematch tabs
cd rematch
ionic platform add android
ionic build android
```

At this point we have created an ionic project using one of the ionic's default template "tabs" and we have compiled our android app. But we need to create a virtual android device. open another console2 window and run

```bash
cd C:\Users\ripu\Desktop\ionic_setup\adt-bundle-windows-x86-20140321\sdk\tools
android avd
```

It should open avd manager, create a virtual device - I used Nexus5 with most of the default options. Try using low configuration so that it will be faster. Now close the AVD manager window and return to the first console window.

```bash
ionic emulate android
```

You should see your new app running on emulator, though it might take some time for android to boot. 




















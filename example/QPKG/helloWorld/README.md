# Hello World
This is a Hello World QPKG example. 

The following instructions can help you to build and use this QPKG.

### Setup QDK Environment
Before start to develop your QPKG or use this example, NAS should already setup the QDK environment:

In QTS Desktop, open **App Center**.

Search **QDK** and install the latest version.

### Build
Upload this project to one of your NAS folder.

Login to QNAP NAS and execute **qbuild** command to build this qpkg.

For example:
```
[admin@SW4-TS42 helloWorld]$ pwd
/share/CACHEDEV1_DATA/QDK-Guide/example/QPKG/helloWorld
[admin@SW4-TS42 helloWorld]$ ls
arm-x19/          arm-x41/          build/            icons/            qpkg.cfg          x86/              x86_ce53xx/
arm-x31/          arm_64/           config/           package_routines  shared/           x86_64/
[admin@SW4-TS42 helloWorld]$ qbuild
Creating archive with data files for arm-x19...
Creating archive with control files...
Creating QPKG package...
Creating archive with data files for arm-x31...
Creating archive with control files...
Creating QPKG package...
Creating archive with data files for arm-x41...
Creating archive with control files...
Creating QPKG package...
Creating archive with data files for arm_64...
Creating archive with control files...
Creating QPKG package...
Creating archive with data files for x86...
Creating archive with control files...
Creating QPKG package...
Creating archive with data files for x86_64...
Creating archive with control files...
Creating QPKG package...
Creating archive with data files for x86_ce53xx...
Creating archive with control files...
Creating QPKG package...
[admin@SW4-TS42 helloWorld]$ ls build/
QNAP_HelloWorld_0.6_arm-x19.qpkg         QNAP_HelloWorld_0.6_arm-x41.qpkg         QNAP_HelloWorld_0.6_x86.qpkg             QNAP_HelloWorld_0.6_x86_ce53xx.qpkg
QNAP_HelloWorld_0.6_arm-x19.qpkg.md5     QNAP_HelloWorld_0.6_arm-x41.qpkg.md5     QNAP_HelloWorld_0.6_x86.qpkg.md5         QNAP_HelloWorld_0.6_x86_ce53xx.qpkg.md5
QNAP_HelloWorld_0.6_arm-x31.qpkg         QNAP_HelloWorld_0.6_arm_64.qpkg          QNAP_HelloWorld_0.6_x86_64.qpkg
QNAP_HelloWorld_0.6_arm-x31.qpkg.md5     QNAP_HelloWorld_0.6_arm_64.qpkg.md5      QNAP_HelloWorld_0.6_x86_64.qpkg.md5
[admin@SW4-TS42 helloWorld]$

```

### Installation

After successfully build QPKG.

Download the corresponding QPKG file in **build/** folder to your computer. (depends on the architecture of your QNAP NAS model)

In QTS Desktop, open **App Center**.

Then manual Install the QPKG.

Now you can test this example QPKG and start to develop your own.
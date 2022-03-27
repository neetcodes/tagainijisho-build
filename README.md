# tagainijisho-build
Unofficial unstable Windows builds with recent definitions for the beloved dictionary application

# As a result of the original developer continuing builds, this is archived. Thanks Gnurou!

Original repository: https://github.com/Gnurou/tagainijisho

Visit [releases](../../releases) page for the builds.  
**Warning**: If you are upgrading, please make a backup of your data with the "Export user data" function in the "Program" menu within the application in case you decide to downgrade.

## Changes
Tagainijisho is a great dictionary application, but as you can see in the main page that the latest release happened in March of 2015.  
So, what has changed?
* JMdict definitions are very dynamic, new words and better definitions (this is the main motivation behind this build)
* Qt4 is outdated, new builds use Qt5
* 64 bit build

and some other things...

## Why isn't there an official build?
Main reason is apparently due to a problem with some entries being removed from JMdict, and this affects user lists etc.  
However this has not been a problem in my experience, I assume it will be the same if you are a new user or just do not care. Hear it from the original author [here](https://github.com/Gnurou/tagainijisho/issues/234).

## Build environment
Last build date (hence JMdict version): 12 Sept 2021  
Arch Linux win32 cross-build  
[Latest commit a16d7b8](https://github.com/Gnurou/tagainijisho/commit/a16d7b82002d95365b54b8cd07d4fd80e2b9cfeb)  
GCC 11.1.0  
Mingw-w64 packages have been retrieved from:
* [mingw-w64-archlinux repository](https://sourceforge.net/projects/mingw-w64-archlinux/files/)
* [martchus-ownstuff repository](https://martchus.no-ip.biz/repo/arch/)

The new build had a couple more .dll dependencies than the official build specification:
```
libssp-0.dll
libbrotlicommon.dll
libbrotlidec.dll
libgraphite2.dll
libpcre2-16-0.dll
```

# Awesome WSL - Windows Subsystem for Linux
[![Awesome][awesomelogo]](https://awesome.re)

An Awesome collection of Windows Subsystem for Linux (WSL) information, distributions, and tools.

<img src="https://raw.githubusercontent.com/sirredbeard/Awesome-WSL/master/WSLscreenshot.PNG" height=50% width=50%>

## Contents
- [Overview](#overview)
- [Using WSL](#using-wsl) <br>
          - [The WSL Shell](https://github.com/sirredbeard/Awesome-WSL#the-wsl-shell) <br>
          - [Programming on WSL](https://github.com/sirredbeard/Awesome-WSL#programming-on-wsl) <br>
          - [Web Development on WSL](https://github.com/sirredbeard/Awesome-WSL#web-development-on-wsl) <br>
          - [Other WSL Uses](https://github.com/sirredbeard/Awesome-WSL#other-wsl-uses)
- [Supported WSL Distributions](#supported-distributions) <br>
          - [Ubuntu](https://github.com/sirredbeard/Awesome-WSL#ubuntu) <br>
          - [Debian](https://github.com/sirredbeard/Awesome-WSL#debian) <br>
          - [OpenSUSE / SUSE Enterprise Linux](https://github.com/sirredbeard/Awesome-WSL#opensuse--suse-enterprise-linux) <br>
          - [Kali Linux](https://github.com/sirredbeard/Awesome-WSL#kali-linux) <br>
          - [WLinux](https://github.com/sirredbeard/Awesome-WSL#wlinux) <br>
- [Unofficial WSL Distributions](#unofficial-distributions)
- [WSL Tools](#wsl-tools) <br>
          - [X Servers](https://github.com/sirredbeard/Awesome-WSL#x-servers) <br>
          - [Terminals](https://github.com/sirredbeard/Awesome-WSL#terminals) <br>
          - [Managing WSL Installations](https://github.com/sirredbeard/Awesome-WSL#for-managing-wsl) <br>
          - [WSL Utilities](https://github.com/sirredbeard/Awesome-WSL#wsl-utilities) <br>
          - [WSL-Specific Development Tools](https://github.com/sirredbeard/Awesome-WSL#wsl-specific-development-tools) <br>
          - [Miscellaneous Tools](https://github.com/sirredbeard/Awesome-WSL#miscellaneous-tools)
- [Additional WSL Resources](#additional-resources)
- [Related Projects](#related-projects)
- [More Awesome Lists](#more-awesome)
- [Thanks](#thanks)
- [Intellectual Property Notices](#intellectual-property-notices)

## Overview

### 1. Linux

Linux is a [UNIX-like](https://github.com/sirredbeard/Awesome-UNIX#frequently-asked-questions) [open-source](https://opensource.org/osd) operating system. The core of Linux is a [kernel](https://www.howtogeek.com/howto/31632/what-is-the-linux-kernel-and-what-does-it-do) developed by [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds). Linux also includes a wide array of applications built on top of the kernel, including [web servers](https://www.linux.com/learn/apache-ubuntu-linux-beginners), [compilers](https://gcc.gnu.org), and [e-mail clients](https://wiki.gnome.org/Apps/Geary), developed and contributed to the Linux ecosystem by a worldwide community of programmers. These applications are then assembled together into Linux [distributions](https://en.wikipedia.org/wiki/Linux_distribution) by [companies](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux), [communities](https://www.archlinux.org), and [individuals](http://www.slackware.com).

### 2. Linux Distributions

Unlike Windows or macOS there are many different Linux distributions, each of which is assembled with different approaches to the software selection and implementation. For example, the goal of the non-profit volunteer [Debian Project](https://www.debian.org/devel/constitution) community is to produce a universal free operating system, while the goal of the for-profit SUSE is to provide a [stable enterprise platform](https://www.suse.com). There are also Linux distributions based on other distributions. [Ubuntu](https://www.ubuntu.com) is a distribution based on Debian built by the company Canonical. Kali is a distribution based on Debian built with an emphasis on tools for network security testing. You can see the most popular distributions ranked at [DistroWatch](https://distrowatch.com).

### 3. Windows

[Windows](https://en.wikipedia.org/wiki/Microsoft_Windows) is a family of proprietary operating systems, all of which are developed, marketed, and sold by Microsoft. Currently Windows 10 is Microsoft's flagship operating system. Windows 10 is available for Intel x86-based and arm64-based PCs. The Windows Subsystem for Linux first shipped in [Windows 10 Anniversary Update](https://blogs.msdn.microsoft.com/wsl/2016/07/08/bash-on-ubuntu-on-windows-10-anniversary-update/), version number 1607, in August 2016. WSL can be enabled for free on all versions of Windows 10 after 1607, including Home, Professional, Enterprise, Server, LTSB, and Education. Originally only available for Intel x86-based PCs, Ubuntu 18.04 for arm64 was made available on the Microsoft store in [May 2018](https://twitter.com/TheRealHariP/status/994293523514970112).

### 4. Windows Subsystem for Linux

Windows Subsystem for Linux is a compatibility layer for running Linux binary executables (ELF) natively on Windows 10. No re-compilation or porting is required. WSL provides a Linux-compatible kernel interface developed by Microsoft and allows a user to chose a Linux distribution to install from the Microsoft Store. Linux applications run within the Linux distribution which provides the application's dependencies and package management in a container-like environment. WSL provides an interface to mount drives within WSL. Additional features are planned.

### 5. Emulation

No. Windows Subsystem for Linux is not an emulator or virtualizer like [VirtualBox](https://www.virtualbox.org). WSL executes unmodified Linux ELF64 binaries by operating a Linux kernel interface on top of the Windows kernel in Windows 10. The WSL kernel interface translates Linux system calls from the binaries into Windows system calls and then executes them at native speed. WSL is closer in its approach to [Wine](https://www.winehq.org) which is a compatibility layer to run Windows binaries on Linux by re-implementing Windows system and API calls in libraries.

### 6. Details

You want the gritty details? Here they are:

- [Windows Subsystem for Linux Overview](https://blogs.msdn.microsoft.com/wsl/2016/04/22/windows-subsystem-for-linux-overview/) at MSDN. 
- [WSL File System Support](https://blogs.msdn.microsoft.com/wsl/2016/06/15/wsl-file-system-support/) at MSDN.
- [WSL System Calls](https://blogs.msdn.microsoft.com/wsl/2016/06/08/wsl-system-calls/) at MSDN.
- [Windows and Ubuntu Interoperability](https://blogs.msdn.microsoft.com/wsl/2016/10/19/windows-and-ubuntu-interoperability/) at MSDN.
- [WSL Antivirus and Firewall Compatibility](https://blogs.msdn.microsoft.com/wsl/2016/11/01/wsl-antivirus-and-firewall-compatibility/) at MSDN.
- [WSL Release Notes](https://docs.microsoft.com/en-us/windows/wsl/release-notes) from docs.microsoft.com.
- [Windows Subsystem for Linux Documentation](https://docs.microsoft.com/en-us/windows/wsl/about) from docs.microsoft.com.
- [Windows Subsystem for Linux - Update](https://www.youtube.com/watch?v=PP_T_m0UV9E) from Microsoft Developer YouTube channel. 
- [Windows for Linux Nerds](https://blog.jessfraz.com/post/windows-for-linux-nerds/) from Microsoft developer Jessie Frazelle.

### 7. Installation

- [Windows 10 Installation Guide](https://docs.microsoft.com/en-us/windows/wsl/install-win10) - Microsoft's official guide.
- [Windows 10 Server Installation Guide](https://docs.microsoft.com/en-us/windows/wsl/install-on-server) - Microsoft's official guide for Windows Server.
- [Windows-Subsystem-For-Linux-Setup](https://github.com/michaeltreat/Windows-Subsystem-For-Linux-Setup) - A basic guide for how to get setup with the WSL feature that is included with Windows 10. ![github project][githublogo]

### 8. Use Cases

WSL is undoubtedly a tool for power-users, developers, and *NIX/Linux geeks who want to run Windows. Most of the things you can do with WSL are going to be related to programming, the console, sysadmin, automation, AI/data science, and other geeky things.

### 9. GUI Apps

Yes, a [suprising number](https://github.com/ethanhs/WSL-Programs) of Linux GUI apps can run on WSL even though this is not officially supported by Microsoft. Running a GUI app on Linux though means running an X server on Windows. This must be downloaded, installed, and running for your GUI app to open from WSL. Otherwise it will complain of not finding a display. X servers for Windows include [X410](https://afflnk.microsoft.com/c/1291904/433017/7593?u=https%3A%2F%2Fwww.microsoft.com%2Fp%2Fx410%2F9nlp712zmn9q) 💰 ($5 but very highly recommended), [VcXsrv](https://sourceforge.net/projects/vcxsrv/), or [Xming](https://sourceforge.net/projects/xming/) on Windows 10.

## Using WSL

#### The WSL Shell

- [Everything You Can Do With Windows 10’s New Bash Shell](https://www.howtogeek.com/265900/everything-you-can-do-with-windows-10s-new-bash-shell/)
- [The Unix Workbench](http://seankross.com/the-unix-workbench/) - A book for anyone to get started with Unix/Linux environments.
- [The Art of Command Line](https://github.com/jlevy/the-art-of-command-line) - Master the command line in one page. ![github project][githublogo]
- [The Bash Academy](http://www.bash.academy) - The Bash Academy is an initiative to promote the bash shell language and educate people on its use.
- [Awesome Command Line Apps](https://github.com/herrbischoff/awesome-command-line-apps) [![Awesome][awesomelogo]](https://awesome.re) ![github project][githublogo]

#### Programming on WSL

Every developer has a unique workflow. Windows and WSL enable developers to carefully customize their setup for their unique workflow. The following are different developers' approaches to creating their development environments using WSL and instructions on how to do the same:

- [Epic Development Environment Using Windows Subsystem for Linux](https://medium.com/@johnwoodruff91/epic-dev-environment-with-wsl-dc81e234ae61) - One developer's approach to their development environment using WSL.
- [Setting Up a Programming Environment via Windows 10 Bash](https://www.cs.odu.edu/~zeil/FAQs/Public/win10Bash/) - From the computer science department at Old Dominion University.
- [WSL as a Development Environment](https://github.com/hsab/WSL-config) - From the computer science department at University of Utah. ![github project][githublogo]
- [Using WSL and MobaXterm to Create a Linux Dev Environment on Windows](https://nickjanetakis.com/blog/using-wsl-and-mobaxterm-to-create-a-linux-dev-environment-on-windows) - Another developer's approach using the third-party terminal MobaXterm.
- [Setting up my WSL Environment - Azure CLI, Docker and .NET](http://tattoocoder.com/setting-up-my-wsl-environment-azure-cli-docker-and-net/)
- [ubuntu-win-boostrap](https://github.com/seapagan/ubuntu-win-bootstrap) - A very simple bootstrap script to install some development basic tools on Debian/Ubuntu on WSL. ![github project][githublogo]
- [Castle-Winbuntu](https://github.com/rodtreweek/Castle-Winbuntu) - Another developer's progress on their development environment using WSL. ![github project][githublogo]
- [Badass Terminal](http://jessicadeen.com/tech/badass-terminal-wsl-macos-and-ubuntu-dotfiles-update/)

For more about learning programming generally, visit [curated-programming-resources](https://github.com/Michael0x2a/curated-programming-resources/blob/master/resources.md).

Microsoft makes [free development tools](https://code.visualstudio.com) available, publishes programming guides through [MSDN](https://msdn.microsoft.com/en-us/library/windows/desktop/ff381399(v=vs.85).aspx), and offers courses through [edX](https://www.edx.org/school/microsoft) and [Microsoft Virtual Academy](https://mva.microsoft.com).

#### Web Development on WSL

Because WSL allows developers to run a variety of Linux server applications locally on their Windows machine, WSL is uniquely useful for web, cloud, and other server-side development tasks. The following are different developers' approaches to creating their web development environment using WSL and instructions on how to do the same:

- [We put Linux in your Windows](https://www.youtube.com/watch?v=JZCPYWrTLTg) - YouTube talk by Windows kernel team member Sarah Cooley on WSL for Windows.
- [Setting Up Windows for Web Development](https://blog.cloudboost.io/setting-up-windows-for-web-development-28483d245a82).
- [How to Install LAMP Stack Server on Windows Subsystem Linux](https://medium.com/@ssharizal/how-to-install-lamp-stack-server-on-windows-subsystem-linux-wsl-windows-10-133419c22473).

For more about learning programming, visit [curated-programming-resources](https://github.com/Michael0x2a/curated-programming-resources/blob/master/resources.md).

Microsoft makes [free development tools](https://code.visualstudio.com) available, publishes programming guides through [MSDN](https://msdn.microsoft.com/en-us/library/windows/desktop/ff381399(v=vs.85).aspx), and offers courses through [edX](https://www.edx.org/school/microsoft) and [Microsoft Virtual Academy](https://mva.microsoft.com).

#### Other WSL Uses

- Learning [programming](https://www.codecademy.com), [computer science](https://www.quora.com/Why-should-computer-science-students-use-the-GNU-Linux-operating-system), and [system administration](https://www.linuxfoundation.org/blog/7-steps-to-start-your-linux-sysadmin-career/) generally.
- Building applications for [Azure](https://blogs.technet.microsoft.com/stefan_stranger/2018/03/08/installing-azure-cli-on-debian-gnulinux-for-wsl/), Microsoft's cloud platform.
- Leveraging the power of the shell and scripting to automate your personal workflow, like OCRing and sorting PDFs into folders using [Python](https://www.pyimagesearch.com/2017/07/10/using-tesseract-ocr-python/).
- Replacing Windows shell [with Xfce, Gnome, KDE, or i3.](https://github.com/NathanCastle/BootShellCredentialProvider).
- Running Linux-based server applications like [OpenFOAM](https://openfoam.org/download/windows-10/) and [Wordpress](https://mkaz.blog/wordpress/install-wordpress-on-windows-subsystem-for-linux/) locally for testing purposes.
- Managing your companies' CentOS servers using [Ansible](https://www.jeffgeerling.com/blog/2017/using-ansible-through-windows-10s-subsystem-linux).
- [pWSLinux+K8S: The Interop way](https://medium.com/@hoxunn/wslinux-k8s-the-interop-way-2d98e5b88f08)
- [Vagrant and Windows Subsystem for Linux](https://www.vagrantup.com/docs/other/wsl.html)

## Supported Distributions

#### Ubuntu

Ubuntu is a Linux distribution based on Debian that is produced by [Canonical Ltd.](https://www.ubuntu.com). Ubuntu 16.04 and the more recent Ubuntu 18.04 are both available for WSL from the Microsoft Store.

- [Windows Store Link](https://www.microsoft.com/store/productId/9NBLGGH4MSV6) for Ubuntu 16.04. Supported through April 2021. Very stable but some packages and libraries may be older.
- [Windows Store Link](https://www.microsoft.com/store/productId/9N9TNGVNDL3Q) for Ubuntu 18.04. Most recent update. Newer packages but more likely to encounter bugs. Supported through April 2023.
- [Installing Software](https://help.ubuntu.com/community/InstallingSoftware) guide to using apt from Ubuntu.
- [Ubuntu Server Guide](https://help.ubuntu.com/lts/serverguide/index.html) from Ubuntu.
- Because Ubuntu is based on Debian, many Debian tutorials also apply to Ubuntu.

#### Debian

Debian is a Linux distribution assembled by volunteers with the community [Debian](https://www.debian.org) Project.

- [Windows Store Link](https://www.microsoft.com/store/productId/9MSVKQC78PK6) for Debian Stretch.
- [Debian Reference](https://www.debian.org/doc/manuals/debian-reference/) post-installation guide for Debian users with a focus on the command line from Debian.
- [Package Management](https://www.debian.org/doc/manuals/debian-reference/ch02.en.html) guide to using apt from Debian.
- [WSL Wiki page](https://wiki.debian.org/InstallingDebianOn/Microsoft/Windows/SubsystemForLinux) from Debian.

#### OpenSUSE / SUSE Enterprise Linux

OpenSUSE and SUSE Enterprise Linux are Linux distributions produced by [SUSE Linux GmbH](https://www.opensuse.org) and other companies. Leap is a community-oriented distribution with recent software. SUSE Enterprise Linux is an enterprise-grade commercial distribution with older tested software.

- [Windows Store Link](https://www.microsoft.com/store/productId/9N1TB6FPVJ8C) for OpenSUSE Leap 15.
- [Windows Store Link](https://www.microsoft.com/store/productId/9PMW35D7FNLX) for SUSE Enterprise Linux 15.
- [Managing Software with Command Line Tools](https://doc.opensuse.org/documentation/leap/reference/html/book.opensuse.reference/cha.sw_cl.html) from OpenSUSE.
- [OpenSUSE Reference](https://doc.opensuse.org/documentation/leap/reference/html/book.opensuse.reference/book.opensuse.reference.html).
- [SUSE Linux Enterprise Documentation](https://www.suse.com/documentation/sles-15/index.html) from SUSE.

#### Kali Linux

Kali Linux is a Linux distribution focused on penetration testing based on Debian that is produced by [Offensive Security](https://www.kali.org).

- [Windows Store Link](https://www.microsoft.com/store/productId/9PKR34TNCV07).
- [Kali Linux Official Documentation](https://www.kali.org/kali-linux-documentation/).
- Because Kali is based on Debian, most Debian and Ubuntu documentation also applies to Kali.

#### WLinux

WLinux is a Linux distribution based on Debian that is designed for WSL users by independent open source developers at [Whitewater Foundry](https://www.whitewaterfoundry.com/).

- [WLinux Store Link](https://afflnk.microsoft.com/c/1291904/433017/7593?u=https%3A%2F%2Fwww.microsoft.com%2Fp%2Fwlinux%2F9nv1gv1pxz6p) 💰
- [WLinux GitHub Page](https://github.com/WhitewaterFoundry/WLinux) ![github project][githublogo]
- Because WLinux is based on Debian, most Debian and Ubuntu documentation also applies to WLinux.

## Unofficial Distributions

Unofficial distributions must be installed manually or with tools listed below. They are not available in the Windows Store.

- [miniwsl](https://github.com/0xbadfca11/miniwsl) - A mini Linux distribution for WSL powered by [busybox](https://www.busybox.net). ![github project][githublogo]
- [ArchWSL](https://github.com/yuk7/ArchWSL) - ArchLinux in WSL. ![github project][githublogo]
- [AlpineWSL](https://github.com/yuk7/AlpineWSL) - Alpine in WSL. ![github project][githublogo]
- [windows-subsystem-linux-fedora](https://gitlab.com/gbraad/windows-subsystem-for-linux-fedora) - Fedora in WSL.
- [WSLInstall](https://github.com/Biswa96/WSLInstall) - Install any GNU/Linux distribution userspace in Windows Subsystem for Linux (WSL) with compressed RootFS tarballs, Docker containers, or ISO files. ![github project][githublogo]
- [WSL-DistroLauncher](https://github.com/yuk7/WSL-DistroLauncher) - General purpose WSL installer and launcher. ![github project][githublogo]
- [WSL-Distribution-Switcher](https://github.com/RoliSoft/WSL-Distribution-Switcher) - Scripts to replace the distribution behind WSL with any other Linux distribution published on [Docker Hub](https://hub.docker.com/explore/). Includes alpine, CentOS, Fedora, Clear, and others. ![github project][githublogo]
- [acme-wsl](https://github.com/elrzn/acme-wsl) - Install acme / plan9port on Debian, Ubuntu, or Kali Linux distributions on WSL. 

## WSL Tools

#### X Servers

An X server running on Windows is required for running Linux GUI apps on Windows. See FAQ #9 above.

- [X410](https://afflnk.microsoft.com/c/1291904/433017/7593?u=https%3A%2F%2Fwww.microsoft.com%2Fp%2Fx410%2F9nlp712zmn9q) - X server for Windows 10 on the Microsoft Store. 💰
- [VcXsrv](https://sourceforge.net/projects/vcxsrv/) - X server for Windows with hardware acceleration compiled with Visual Studio.
- [Xmanage](https://www.netsarang.com/products/xmg_overview.html) - X server for Windows from NetSarang. 💰
- [Xming](https://sourceforge.net/projects/xming/) - An older X server for Windows. Has not been updated since 2016.
- [Cygwin/X](https://x.cygwin.com) - Cygwin/X is a port of the X Window System to the Cygwin API layer for Windows.

#### Terminals

- [wsltty](https://github.com/mintty/wsltty) - Mintty as a terminal for WSL. ![github project][githublogo]
- [wsl-terminal](https://github.com/goreliu/wsl-terminal) - A terminal emulator for WSL, based on mintty, fatty and wslbridge. ![github project][githublogo]
- [Terminus](https://eugeny.github.io/terminus/) - A terminal for a more modern age. ![github project][githublogo]
- [ConEmu](https://conemu.github.io) - ConEmu aims to be handy, comprehensive, fast and reliable terminal where you may host any console application for the Windows command line, PowerShell, or WSL. 
- [MobaXterm](https://mobaxterm.mobatek.net) - Enhanced terminal for Windows with X11 server, tabbed SSH client, network tools and much more.
- [extraterm](https://github.com/sedwards2009/extraterm) - Open source project to build a terminal emulator and expand it with new features to support modern workflows. ![github project][githublogo]
- [Hyper](https://hyper.is/) - A terminal built on web technologies. ![github project][githublogo]

#### For Managing WSL Installations

- [LxRunOffline](https://github.com/DDoSolitary/LxRunOffline) - A full-featured utility for managing WSL. ![github project][githublogo]
- [wslu](https://github.com/patrick330602/wslu) - A collection of utilities for Windows 10 Linux Subsystem, such as enabling sound in WSL and creating your favorite linux GUI application shortcuts on Windows 10. ![github project][githublogo]
- [Ansible-WSL](https://github.com/Wintus/Ansible-WSL) - Provision WSL using Ansible. ![github project][githublogo]

#### WSL Utilities

- [wslgit](https://github.com/andy-5/wslgit) - Use git installed on WSL from Visual Studio Code on Windows. ![github project][githublogo]
- [wsl-proxy](https://github.com/watzon/wsl-proxy) - A collection of 'proxy' batch files that can be used to route requests to the WSL version of a command. ![github project][githublogo]
- [wslpath](https://github.com/laurent22/wslpath) - Easily convert Windows to WSL path names and vice-versa. ![github project][githublogo]
- [wsl-open](https://github.com/4U6U57/wsl-open) - Open files with xdg-open in WSL from Windows applications. ![github project][githublogo]
- [is-wsl](https://github.com/sindresorhus/is-wsl) - Check if the current process is running inside Windows Subsystem for Linux, useful for scripting. (Node implementation)![github project][githublogo]
- [is_wsl](https://github.com/julien-h/is-wsl) - Check if the current process is running inside Windows Subsystem for Linux, useful for scripting. (Python implementation)![github project][githublogo]

#### WSL-Specific Development Tools

- [wsl-docker-git-setup](https://github.com/rodtreweek/Castle-Winbuntu) - Shell script to configure WSL to use docker and docker-compose as well as a git-enabled prompt. ![github project][githublogo]
- [ghc](https://launchpad.net/~hvr/+archive/ubuntu/ghc-wsl) - A version of the Glasgow Haskell Compiler built and optimized for WSL and hosted in a PPA for Debian and Ubuntu-based WSL distros.

#### Miscellaneous Tools

- [BootShellCredentialProvider](https://github.com/NathanCastle/BootShellCredentialProvider) - BSCP lets you boot Windows directly into a Linux desktop experience such as xfce4 using Windows native login and a combination of Xming & WSL upon login. ![github project][githublogo]
- [wsl-dotfiles](https://github.com/Xyene/wsl-dotfiles) - Configuration files and scripts for creating an i3-based environment inside WSL. ![github project][githublogo]
- [EnumWSL](https://github.com/therealkenc/EnumWSL) - Enumerates installed WSL packages. ![github project][githublogo]
- [WSL-DistroLauncher](https://github.com/Microsoft/WSL-DistroLauncher) - Reference launcher app for developing your own WSL distribution Microsoft Store package. ![github project][githublogo]
- [WSL_Reverse](https://github.com/Biswa96/WSL_Reverse) - Reveal hidden COM interface between WSL and Lxss Manager Service. ![github project][githublogo]
- [wslbridge](https://github.com/rprichard/wslbridge) - wslbridge is a Cygwin program that allows connecting to the WSL command-line environment over TCP sockets, as with ssh, but without the overhead of configuring an SSH server. ![github project][githublogo]
- [WSLInstall](https://github.com/Biswa96/WSLInstall) - Install any Linux distribution userspace in WSL with compressed RootFS tarballs (tar.gz) or with Docker containers or with ISO files. ![github project][githublogo]
- [cmd-colors-solarized](https://github.com/neilpa/cmd-colors-solarized) - This is a solarized color scheme for the Windows command prompt that works in WSL.

## Additional Resources

- Microsoft [WSL Blog](https://blogs.msdn.microsoft.com/wsl)
- Microsoft [Console Blog](https://blogs.msdn.microsoft.com/commandline/)
- [WSL-Programs](https://github.com/ethanhs/WSL-Programs) - A community powered list of programs that work on the Windows Subsystem for Linux. ![github project][githublogo]
- [/r/bashonubuntuonwindows](https://www.reddit.com/r/bashonubuntuonwindows/) - Reddit subreddit.
- [##windows-wsl](https://irc-source.com/channel/freenode/%23%23windows-wsl) - IRC channel on Freenode.net. 
- [#debian-wsl](https://www.oftc.net) - IRC channel on OFTC.net.
- [WSL on GitHub](https://github.com/Microsoft/WSL) - For reporting issues with WSL. ![github project][githublogo]
- [The Windows Subsystem for Linux Guide](http://wsl-guide.org/en/latest/) - Third-party WSL resource.
- [Microsoft User Voice](https://wpdev.uservoice.com/forums/266908-command-prompt-console-bash-on-ubuntu-on-windo/category/161892-bash) - Send Microsoft feedback on WSL.
- [Microsoft Developer Feedback](https://wpdev.uservoice.com/forums/266908-command-prompt-console-windows-subsystem-for-l) - For developers to send Microsoft feeback on WSL.
- [Stack Overflow: WSL](https://stackoverflow.com/questions/tagged/wsl) - Programming question and answer site.

## Related Projects

- [Bash](https://www.gnu.org/software/bash/) - Bash is the GNU Project's shell. Bash is the Bourne Again SHell. Bash is an sh-compatible shell that incorporates useful features from the Korn shell (ksh) and C shell (csh).
- [Cygwin](https://cygwin.com) - Cygwin is a Unix-like environment and command-line interface for Microsoft Windows.
- [Babun](http://babun.github.io) - A Linux-like console on a Windows host. ![github project][githublogo]
- [PuTTY](https://www.putty.org) - PuTTY is an SSH and telnet client, developed originally by Simon Tatham for the Windows platform. ![github project][githublogo]
- [PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6) - PowerShell is a task automation and configuration management framework from Microsoft, consisting of a command-line shell and associated scripting language.
- [Visual Studio Code](https://code.visualstudio.com) - Visual Studio Code ("vscode") is a source code editor developed by Microsoft for Windows, Linux, and macOS. It includes support for debugging, embedded Git control, syntax highlighting, intelligent code completion, snippets, and code refactoring.
- [Visual Studio 2017](https://www.visualstudio.com/vs/) - Visual Studio is an IDE from Microsoft. It is used to develop computer programs, as well as web sites, web apps, web services and mobile apps. Visual Studio uses Microsoft software development platforms such as Windows API, Windows Forms, Windows Presentation Foundation, Windows Store, and Microsoft Silverlight.
- [Windows Services for UNIX](https://en.wikipedia.org/wiki/Windows_Services_for_UNIX) - SFU is a discontinued software package produced by Microsoft which provided a Unix environment on Windows NT and some of its immediate successor operating-systems. [TechNet](https://technet.microsoft.com/en-us/library/bb496506.aspx) documentation.

## More Awesome

- [Awesome UNIX](https://github.com/sirredbeard/Awesome-UNIX)
- [Awesome Windows](https://github.com/Awesome-Windows/Awesome)
- [Awesome VSCode](https://github.com/viatsko/awesome-vscode)
- [Awesome Bash](https://github.com/awesome-lists/awesome-bash)
- [Awesome Shell](https://github.com/alebcay/awesome-shell)
- [Awesome Powershell](https://github.com/janikvonrotz/awesome-powershell)
- [Awesome Linux](https://github.com/aleksandar-todorovic/awesome-linux)

More [![Awesome][awesomelogo]](https://awesome.re) lists. ![github project][githublogo]

## Thanks

- The Windows 10, WSL, and kernel teams at Microsoft, including but not limited to [Tara Raj](https://twitter.com/tara_msft), [Rich Turner](https://twitter.com/richturn_ms), [Jessie Frazelle](https://twitter.com/jessfraz), [Jack Hammons](https://github.com/jackchammons), [Sarah Cooley](https://github.com/scooley), [Ben Hillis](https://github.com/benhillis), [Allen Sudbring](https://blogs.technet.microsoft.com/askpfeplat/tag/allen-sudbring/), [Brandon Wilson](https://social.technet.microsoft.com/profile/BrandonWilson), [John Starks](https://twitter.com/gigastarks), [Russ Alexander](https://www.linkedin.com/in/russalex), [Yosef Durr](https://twitter.com/yosefdurr), [Sven Groot](https://twitter.com/svengroot_ms), [Sunil Muthuswamy](https://twitter.com/SunilMut), [Palkesh Soni](https://twitter.com/sonipalkesh), [John Starks](https://twitter.com/gigastarks), [Craig Wilhite](https://twitter.com/CraigWilhite).
- [Canonical](https://www.ubuntu.com), [Debian](https://www.debian.org), [SUSE](https://www.suse.com), and [Offensive Software](https://www.offensive-security.com).
- The [Awesome community](https://awesome.re) on GitHub.

## Intellectual Property Notices

- Linux® is a registered trademark of Linus Torvalds in the United States and/or other countries. [*](https://www.linuxfoundation.org/trademark-usage/)
- Windows®, Windows Server®, Windows 10®, Microsoft®, Microsoft Virtual Academy®, Visual Studio®, Azure®, PowerShell®, and MSDN® are trademarks or registered trademarks of Microsoft Corporation in the United States and/or other countries. [*](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general.aspx) [**](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/en-us.aspx)
- EdX® is a registered trademark of edX Inc. All Rights Reserved. [*](https://www.edx.org/trademarks)
- Ubuntu® and Canonical® are registered  trademark of Canonical Limited in the United States and/or other countries. [*](https://www.ubuntu.com/legal/terms-and-policies/intellectual-property-policy)
- SUSE® and SUSE Linux Enterprise® are registered trademarks of SUSE in the United States and/or other countries. [*](https://www.suse.com/company/legal/)
- Red Hat®, CentOS®, and Red Hat Enterprise Linux® are trademarks or registered trademarks of Red Hat, Inc. in the United States and/or other countries. [*](https://www.redhat.com/en/about/trademark-guidelines-and-policies)
- UNIX® is a trademark of The Open Group. Use of The Open Group trademarks are authorized by The Open Group Trademark Guidelines as "Editorial or Articles, but not Advertising" and/or permitted by trademark fair use under United States law. [*](http://www.unix.org/trademark.html)
- Debian® is a registered trademark of Software in the Public Interest, Inc. in the United States and/or other countries. [*](https://www.debian.org/trademark)
- Kali Linux® and Offensive Security® are registered trademarks of OffSec Services, Ltd. [*](https://www.offensive-security.com/trademark-policy/)
- Docker® and Docker Hub® are registered trademarks of Docker, Inc. [*](https://www.docker.com/trademark-guidelines)
- YouTube® is a registered trademark of Google, LLC. [*](https://www.google.com/permissions/trademark/our-trademarks.html)
- macOS® is a registered trademark of Apple, Inc. [*](https://www.apple.com/legal/intellectual-property/guidelinesfor3rdparties.html)
- GitHub® and [githublogo] are a registered trademarks of GitHub, Inc. [*](https://help.github.com/articles/github-terms-of-service/)
- Oracle and Oracle Linux are trademarks or registered tracemarks of Oracle, Inc. [*](https://www.oracle.com/legal/trademarks.html)

All other trademarks mentioned herein are the property of their respective owners and may be registered in the United States and/or other countries.

The author of this project has no connection with Microsoft, Inc.

Portions of the descriptions above are from Wikipedia and used under [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/). Portions of the descriptions above are from [Awesome-UNIX](https://github.com/sirredbeard/Awesome-UNIX) and used under [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).

This document is licensed under [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).

[githublogo]:https://raw.githubusercontent.com/sirredbeard/Awesome-WSL/master/github-icon.png
[awesomelogo]:https://awesome.re/badge.svg

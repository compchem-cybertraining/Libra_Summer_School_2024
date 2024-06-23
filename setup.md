---
title: Setup
---

<a name="toc"></a>
Table of Contnet 

1. [Getting the CCR accounts and VPN](#1)
2. [Libra](#2)
3. [Terminal](#3)
4. [Text editors](#4)
5. [Molecular visualization and editing tools](#5)



<a name="1"></a>[Back to TOC](#toc)
# 1. Getting the CCR accounts and VPN

Below are the steps you’ll need to take to get the accounts setup. This is a little confusing because you actually have two accounts.
One is an account that gets you access to the University at Buffalo’s VPN network and the other is the account you’ll use to access CCR’s cluster.
Please **read these steps and the instructions on the links shared here carefully.**  If you run into trouble, I recommend reviewing the steps again 
to ensure you completed them all. If you have questions or problems, please contact ccr-help@buffalo.edu. 

 
## Step 1:  Setup two factor authentication for your UB VPN account. 

The username for this account is: **given to you by the CCR staff**

Password: **sent in a separate email**

Instructions can be found [here](https://ubccr.freshdesk.com/support/solutions/articles/13000094126-external-collaborator-industry-business-customer-access)

 
## Step 2:  In order to connect to our machines, you have to be on the UB network.  You'll need to download and install **UB's Cisco VPN client.** 
You will be receiving a separate email from Globus with the link to download this software.  If you do not already have a Globus account, 
you will be instructed to create one at this point.  The UB account will not work for the Globus service. 

NOTE: this link is only accessible using the email address this is getting sent to. 
 

## Step 3:  Connect to the CCR VPN – instructions are in the first link above.

When you start the Cisco software the first time you will need to enter the following in the "Connect to:" box: vpn.buffalo.edu and then 
select CCR from the group drop down menu.  Enter the UB VPN username and password from above and use Duo as your two step verification.

Now that you have setup the UB account and connected to the VPN, you’ll be able to move forward with your CCR account. 
 

## Step 4 (optional): If you’re unsure of your CCR account password you can reset it. Make sure you’re connected to the UB VPN and go to 
[CCR’s identity management portal](https://idm.ccr.buffalo.edu), enter your CCR username and click the Next button.
Then click the “forgot your password?” link to generate a one-time password reset link.  The link contained in this email only lasts for 15 minutes. 

Your account has two factor authentication enabled.  If you have trouble remembering how to use it, please refer 
to [the documentation](https://docs.ccr.buffalo.edu/en/latest/2fa/)

 
## Step 5: FINALLY…Connect to CCR!

There are two ways to connect to our systems:

    * [OnDemand web portal](https://ondemand.ccr.buffalo.edu)

    * If you choose to use a SSH client, you may login to our pool of front end servers with the address: vortex.ccr.buffalo.edu.  
      You must use SSH keys as we do not accept passwords over SSH.  We have information about this [here](https://docs.ccr.buffalo.edu/en/latest/hpc/login/)

All documentation for using our systems can be found [here](https://docs.ccr.buffalo.edu)


<a name="2"></a>[Back to TOC](#toc)
# 2. Libra and other Python libraries

This workshop will be focused on the [Libra](https://github.com/Quantum-Dynamics-Hub/libra-code/tree/devel) package developed by the 
[Akimov group](https://akimovlab.github.io/). 

Although Libra and some of its strong and weak dependencies are already installed on UB CCR and will be directly accessible via
the Jupyter notebooks on OnDemand, you may want/need to install them locally. Since most of the calculations we'll be doing 
are not too intensive computationally, runnig most of them on your laptop shall not be a problem. 

You may want to use this option, if you want to follow the hands-on exercises with Libra, but you have not been accepted as a fully-fledged 
participant (the participant without full access to UB CCR resources, which may be because of your geographic location at the moment).

Please follow the [installation instructions](https://github.com/Quantum-Dynamics-Hub/libra-code/tree/devel) to build the corresponding 
environment, install all needed dependencies and packages, and build and install the Libra code itself. **Make sure to use the "devel" branch**. 


<a name="3"></a>[Back to TOC](#toc)
# 3. Terminal 

The terminal is an interface in which you can type and execute text based commands. It is important to use the terminal to 
run many computational chemistry software packages. There are several different types of terminal interfaces, called shells.
In this tutorial, we will focus on using one of the most common shells, the bash shell. 
How you acquire a bash shell terminal depends on the type of computer you have.

## 3.1. Linux
If you are using a Linux computer, you probably already know how to open the terminal window. 
If the Terminal is not shown in menu of programs, you can use the key combination CTRL + ATL + T to open the terminal window.

## 3.2. Mac OS X
On Mac OS X, a Terimanl application is built into your system. Open the Terminal from Applications -> Utilities -> Terminal.

## 3.3. Windows 11
Windows has a built in command line interface. To access it, click the Windows Key + R, type cmd, press Enter.
**However,** this interface is not a bash application. Therefore, the commands for navigating and creating files discussed below
 will not be the same. We recommend you installing the [Windows Subsystem for Linux](https://devblogs.microsoft.com/commandline/learn-about-windows-console-and-windows-subsystem-for-linux-wsl/) instead. Please follow [these instructions](https://docs.microsoft.com/en-us/windows/wsl/install-win10) to install 
 it for your system. This will allow you having a fully-fledged Linux/Unix terminal experience while still working on Windows 10.

## 3.4. Resources
- [Using the command line](https://ryanstutorials.net/linuxtutorial/commandline.php)
- [Navigation in bash](https://ryanstutorials.net/linuxtutorial/navigation.php)
- [Making and removing directories, copying and deleting files](https://ryanstutorials.net/linuxtutorial/filemanipulation.php)


<a name="4"></a>[Back to TOC](#toc)
# 4. Text Editors

You will often need to create or read text files.  Opening a text file in a word processing program,
like Microsoft Word or Google Docs, introduces a lot of formatting that is not needed. 
You need to use a text editor to read and write these files. There are many choices. You don't need to learn to 
use all of these at the beginning, just find one that works for you. 

## 4.1. Vi/vim
Vi/vim is one of the most ubiquitous text editors. It is installed on virtually every Linux computer in the world, 
so if you ever log on to a unfamiliar machine, it will be available to you. 
Vi is accessed from the command line; it doesn't have or need a graphical interface so it can operate on the most bare bones computers.
However, it is not intuitive to use and can be difficult for beginners.
- [Interactive vim tutorial](https://www.openvim.com/)
- [Getting started with vi](https://ryanstutorials.net/linuxtutorial/vi.php)

## 4.2. Far 3
[Far3](https://www.farmanager.com/) is a very handy file and archive manager. Features rather convenient graphical interface and some
convenient manipulation options such as cutting any blocks of text, syntax highlightling, remote drive access, etc. Don't get
scared by its old-style "Norton/Midnight Commander" look. You'll love it. If you run Windows, this is definitely our recommendation. 

![](/fig/setup/far.png){:width="80%"}


## 4.3. Atom
[Atom](https://atom.io/) is a modern text editor that is very intuitive to use. You probably don't even need 
to read the tutorial below to figure out how to create and save files. Standard downloads are available for Linux, Mac, and Windows.
- [Getting started with atom](https://flight-manual.atom.io/getting-started/sections/atom-basics/)

## 4.4. Emacs
Similar to vi/vim, emacs is a command line text editor that is already part of almost all Linux distributions.
Emacs can also be used as an RSS reader or file manager.
- [Emacs tutorial](https://www.gnu.org/software/emacs/tour/) The section called Beginner tips near the bottom of the page is particularly helpful.

## 4.5. Sublime
[Sublime](https://www.sublimetext.com/) is an intuitive text editor that makes looking at files with multiple sections easy. 
t allows split screen editing and is very customizable.


<a name="5"></a>[Back to TOC](#toc)
# 5. Molecular visualization and editing tools

|   |   |
|---|---|
| [VESTA](https://jp-minerals.org/vesta/en/) | ![](/fig/setup/vesta.png){:width="80%"} | [Tutorials by Brendan Smith](https://github.com/compchem-cybertraining/Tutorials_Editing_Visualization) |
| [VMD](https://www.ks.uiuc.edu/) | ![](/fig/setup/vmd.png){:width="80%"} |
| [IQmol](http://iqmol.org/)  | ![](/fig/setup/IQmol.png){:width="80%"} | [Tutorial by Alexey Akimov](https://youtu.be/BXtPtkUJVqc) |
| [Avogadro](https://avogadro.cc/) | ![](/fig/setup/avogadro.png){:width="80%"} |





{% include links.md %}

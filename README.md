<!---
This document is the README.md for a code repoitory hosted free on GitHub.
This document is from the repository "CyberWM-Dark" by User: "tREEs-Repos"
This document will be shown on the main page of the repository.
It is written with Markdown Formatting.

Repository URL:
https://github.com/tREEs-Repos/CyberWM-Dark/
--->

<!--- Start the README with some markdown badges Indicating the Supported Platforms --->
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![FreeBSD](https://img.shields.io/badge/-FreeBSD-%23870000?style=for-the-badge&logo=freebsd&logoColor=white)
![XFCE](https://img.shields.io/badge/XFCE-%232284F2.svg?style=for-the-badge&logo=xfce&logoColor=white)

<!--- Display the README banner image as the document Title --->
![README Banner](banner.png)

<!--- Interactive Table of Contents leading to Headers in the Document --->
## Table of Contents
- [Description](#project-description)
- [Themes And Previews](#themes-and-previews)
- [Installation](#installation)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Bugs and Feedback](#bugs-and-feedback)

<!--- A Brief Summary of the Project and what functionality it provides / goal it accomplishes --->
### Project Description:
The 'Cyber-WM Dark' theme collection is a variety of dark-mode styles for the XFCE Window Manager. This repository comes with 11 
color styles to choose from, making it even more likely you'll find a color to make your build stand out.

Experience a unique GUI feel with CyberwMs use of Shadow Effects which appear to change your Window shape entirely when in 
windowed mode. 

CyberWM is ported from 'ghost-dark', a Window Manager style by [Purnomoshinigami](https://www.xfce-look.org/u/purnomoshinigami).

It is originally inspired by the ColdSteel Oroborous Theme. 

<!--- Preview Images of each Theme Color. --->
<!--- Preview Images are stored in the root directory of each individual Theme. --->
## Themes and Previews
This theme collection comes in 11 color combinations. These are listed below, in the order they appear in the Repository files.

* CyberWM-Dark-DeepBlue
  ![Deep Blue Preview](CyberWM-Dark-DeepBlue/preview.png)

* CyberWM-Dark-DeepPurple
  ![Deep Purple Preview](CyberWM-Dark-DeepPurple/preview.png)

* CyberWM-Dark-Gray
  ![Gray Preview](CyberWM-Dark-Gray/preview.png)
  
* CyberWM-Dark-Green
  ![Green Preview](CyberWM-Dark-Green/preview.png)

* CyberWM-Dark-LightBlue
  ![Light Blue Preview](CyberWM-Dark-LightBlue/preview.png)

* CyberWM-Dark-LightPurple
  ![Light Purple Preview](CyberWM-Dark-LightPurple/preview.png)

* CyberWM-Dark-Midnight (*All Black*)
  ![Midnight Preview](CyberWM-Dark-Midnight/preview.png)

* CyberWM-Dark-Pink
  ![Pink Preview](CyberWM-Dark-Pink/preview.png)

* CyberWM-Dark-Red
  ![Midnight Preview](CyberWM-Dark-Red/preview.png)

* CyberWM-Dark-White
  ![Midnight Preview](CyberWM-Dark-White/preview.png)

* CyberWM-Dark-Yellow
  ![Midnight Preview](CyberWM-Dark-Yellow/preview.png)

<!--- Section for Installation techniques and Explanation --->
## Installation
<!-- The Introduction tries to help users locate the correct path for the Installation --->
To Install  this theme collection. You will first need to know where your system stores XFCE Themes.

There are multiple ways to do this and it is up to the user to work out the correct path themselves.

Some common locations for theme configurations are:

* `/usr/share/themes/`
* `/usr/share/xfwm4/themes/`
* `~/.themes/`
* `~/.local/share/themes/`

For the purposes of this guide we will be installing to the most standard location. `/usr/share/themes/`
We will also assume you have knowledge of using `git` and basic system utilities.

<!--- This Section Signposts Users to different parts of the Installation Guide. --->
### Installation Options:
- [Installing the Full Theme Collection](#approach-1-installing-the-full-theme-collection)
- [Installing Individual Themes](#approach-2-installing-individual-themes)
- [Previewing your Theme before use](#previewing-your-theme-before-use)
- [Using your Theme](#using-your-theme)
- [Clean Uninstall](#how-to-uninstall-cleanly)

___

<!--- Guide for Approach: Installing the Full Theme Collection --->
### **APPROACH 1: INSTALLING THE FULL THEME COLLECTION**
This is the simplest approach to Installation and installs every color variant on your system.

1. First, clone this repository in a location of your choice.
   ```
   # Command 1 - Enter the Directory to store the repo files in.
   cd ~/Downloads

   # Use 'git' to clone the repository from Github.
   git clone https://github.com/tREEs-Repos/CyberWM-Dark
   ```

   You should see similar output to this:
   ```
   Cloning into 'CyberWM-Dark'...
   remote: Enumerating objects: 353, done.
   remote: Counting objects: 100% (353/353), done.
   remote: Compressing objects: 100% (108/108), done.
   remote: Total 353 (delta 257), reused 320 (delta 242), pack-reused 0 (from 0)
   Receiving objects: 100% (353/353), 3.21 MiB | 5.73 MiB/s, done.
   Resolving deltas: 100% (257/257), done.
   ```

2. Enter the Downloaded Repo and transfer all the root directory subfolders to your install location.
   ```
   # Enter the Downloaded Repository Directory
   cd CyberWM-Dark/ 
   ```

   You now have two options. If you want to transfer the themes directly without preserving the source use `mv`.

   This operation may need `sudo` permissions on some machines if moving files to the rootfs.
   ```
   # Move all Subfolders to /usr/share/themes.
   # This command only moves Directories beginning with CyberWM-Dark
   sudo mv -v CyberWM-Dark*/ /usr/share/themes
   ```

   If you are successful you should see output like this:
   ```
   renamed 'CyberWM-Dark-DeepBlue/' -> '/usr/share/themes/CyberWM-Dark-DeepBlue'
   renamed 'CyberWM-Dark-DeepPurple/' -> '/usr/share/themes/CyberWM-Dark-DeepPurple'
   renamed 'CyberWM-Dark-Gray/' -> '/usr/share/themes/CyberWM-Dark-Gray'
   ...
   ```

   If you wish to save a copy of the source files, then use the `cp` utility.

   This operation may need `sudo` permissions on some machines if copying files to the rootfs.
   ```
   # Copy all subfolders to /usr/share/themes
   # This command also only moves directories beginning with CyberWM-Dark
   sudo cp -rv CyberWM-Dark*/ /usr/share/themes
   ```

   If you are successful you should see output like this:
   ```
   'CyberWM-Dark-DeepBlue/' -> '/usr/share/themes/CyberWM-Dark-DeepBlue'
   'CyberWM-Dark-DeepBlue/README.md' -> '/usr/share/themes/CyberWM-Dark-DeepBlue/README.md'
   'CyberWM-Dark-DeepBlue/preview.png' -> '/usr/share/themes/CyberWM-Dark-DeepBlue/preview.png'
   ```

4. Your Theme is now Installed. Easy, right?
    
   See how to: [Preview your Theme](#previewing-your-theme-before-use) or jump right in to [using](#using-your-theme) it!

   Errors / Issues on our side? Please see the section on how to leave Feedback: [Bugs and Feedback](#bugs-and-feedback).

   Wish to uninstall? Please check [the Removal Guide](#how-to-uninstall-cleanly).


### APPROACH 2: INSTALLING INDIVIDUAL THEMES

### PREVIEWING YOUR THEME BEFORE USE

### USING YOUR THEME

### HOW TO UNINSTALL CLEANLY

___

<!--- Including a copy of the Creative Commons Zero License in the README for Transparency --->
## License
The CyberWM Theme Collection is Provided under the Creative Commons Zero License. 
A copy of the license is included below in full:

```
________________________________________________________________________________________
This license description applies to: "CyberWM-Dark XFCE Window Manager Themes" by tREEs
The full repository is available at this URL: https://github.com/tREEs-Repos/CyberWM-Dark
_________________________________________________________________________________________

____________________________________________________
CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
____________________________________________________

The person who associated a work with this deed has dedicated the work to the public domain 
by waiving all of his or her rights to the work worldwide under copyright law, including all 
related and neighboring rights, to the extent allowed by law.

You can copy, modify, distribute, and perform the work, even for commercial purposes, all 
without asking permission. Full Copy of the legal code: 

https://creativecommons.org/publicdomain/zero/1.0/legalcode

By using this code repository you agree to be bound by the conditions of this license.
_________________________________________________________________________________________
```
A copy of the License will be cloned with the Repository. It is available ![here](https://github.com/tREEs-Repos/CyberWM-Dark/blob/main/LICENSE.txt).

<!--- Repository Acknowledgements --->
## Acknowledgements

**Purnomoshinigami** - An Indonesian user on XFCE Look.
He has some amazing Window Manager themes that seem to turn up on all my XFCE Builds.
Support him by checking out his ![XFCE Look](https://www.xfce-look.org/u/purnomoshinigami) Account and seeing if theres anything you like.

**XFCE-Look.org** - 
A well known, leading source of configurations for XFCE, GTK, Compix, Beryl / Emerald Themes and more.
Support the website by checking it out and seeing if theres anything you like.
The XFCE-Look website is linked directly ![here](https://www.xfce-look.org/).

## Bugs and Feedback
Issues / Errors with this Repository? Reach out here via Github.

Feedback? Also feel free to reach out here via Github. Your input is always appreciated!

I am always open to requests to refactor and redesign this repository if you have a better system.
___

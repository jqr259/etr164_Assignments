# Final Project Documentation
&nbsp;
### Project Goal
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The goal of this project was to create a custom linux distribution aimed at providing software and resources for monitoring and diagnosing hardware failures.

### Getting Started
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After doing extensive research on the feasibility of one of my original goals, using software (perhaps creating custom software) to diagnose the problems with faulty hardware pieces, I had a realization and had to change course slightly. So instead of using a piece of software to analyze the direct issue it was now apparent to me that I needed to use the process of elimination to rule out the functioning parts and therefore isolating the bad part or parts.  What this entails is using Stress Testing on each part individually to ensure each one works the way it was intended thus being able to cross that piece off as the root of the problem.  There are certainly limitations to this, i.e. you can't really stress test a power supply, but you can get a general idea of where to start looking.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;So my new goal became to create a distro that had the necessary tools to test each component possible, and to use monitoring tools to measure the results.
### The first steps & Installation
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The first few attempts at this didn't go well, the first linux distribution I tried to use as a base was Ubuntu 14.04 because it was the last version of Ubuntu that had a compatible version of the Ubuntu Customisation Kit (UCK), which was a tool that allowed you to select which packages you wanted installed, and then roll your own install and setup into an iso that you could install elsewhere or distribute.  However 14.04 didn't work because it wasn't easily compatible with newer computers and in particular newer graphics cards.  Next I tried Ubuntu 16.04, 17.10 and Linux Mint because I had experience with using them however I found it extremely difficult to manually get rid of all of the packages I didn't want, as well as repeatedly running into issues with booting from a flash drive (in hindsight I was probably also causing some compatibility issues with the necessary software).  After that I briefly flirted with the idea of using Arch linux, because of the total control you get over the system, however, that was short lived as I was never able to get it fully installed.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After crawling through forums I came across a suggestion to use a server version of Ubuntu as an alternative to removing packages from a full install because it gives you the option to start from the bare minimum and work your way up from the ground.  After creating a bootable usb with the 18.04 server iso on it I plugged both flash drives in and restarted my computer.  When the computer restarted I booted from the usb with the iso already on it and went through the installation process, which was fairly straightforward with the exception of partitioning the other flashdrive manually as the installation destination.  After it installed I turned on the universe repository, as well as adding a few more here and there as needed, and went about installing some basic commands that don't come installed.  After that I installed both NVIDIA and AMD's proprietary graphics drivers, followed by installing a light weight desktop environment, Xfce.  After that was finished I went on installing the software needed to monitor and stress test computers (see next section).

### Software Used
- Ubuntu Server 18.04
- Xfce desktop environment
- Mozilla firefox
- memtest86+
- Prime95
- GLmark2
- smartmontools
    - smartctl
- Conky
- HWinfo

### Results
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Unfortunately much to my dismay I ran into compatibilty issues with running this system on machines other than my desktop which I installed it from.  This was a huge let down for me because I thought I had finally found something that worked and that I had it at a stage where I could start testing it on computers with bad parts.  Regrettably this was as far as I was able to get with this project as I was never able to find a solution to the problems I was having trying to boot from other computers.

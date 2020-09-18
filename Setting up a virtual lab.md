# Setting up a lab 
We need to setup a virtual lab so that our acts wont affect our main system or may not harm our main system while we conduct any test as handling of some potentially dangerous malwares may be needed at certain stages. 
To set up a lab we will be using kali linux/Parrot Sec OS.
We are going to set up a virtual lab refer to the section which belongs to your system OS. 


## 1. Downloading and Installing Virtual Box


## Windows OS users
 Make sure your computer’s hardware virtualization settings are enabled in your BIOS settings. Most current PCs should have it enabled, but if you are 
 using an older computer or are having issues running virtual machines, you may have to enable this setting. (You will have to Google your model computer to see how 
 to turn this on) Most people recommend 4GB of RAM, but I usually make sure I have at least 8-10GB of RAM. This makes sure you have enough RAM to run your host and guest
 operating systems smoothly.Make sure you have enough hard drive space on your host computer to install each virtual machine. The sizes of memory on each virtual machine is
 different, so make sure your hard drive has room if you plan on installing several at a time.
    
This section here belongs and shows how to set up a virtual lab in windows machine.
 
 ## Steps
 1. Open the VirtualBox website. Go to https://www.virtualbox.org/ in your computer's Internet browser. This is the website from which you'll download the VirtualBox 
 setup file. 
 
 2. Click Download VirtualBox. It's a blue button in the middle of the page. Doing so will open the downloads page. 
 
 3. Click Windows hosts. You'll see this link below the "VirtualBox 6.1 platform packages" heading. The VirtualBox EXE file will begin downloading onto your computer. 
 
 4. Open the VirtualBox EXE file. Go to the location to which the EXE file downloaded and double-click the file. Doing so will open the VirtualBox installation window.
 
 5. Navigate through the installation prompts. Do the following:

    Click Next on the first three pages.
    Click Yes when prompted.
    Click Install
    Click Yes when prompted.

6.Click Install when prompted. Doing so will allow VirtualBox to begin installing on your computer. 

7.Click Finish when prompted. It's in the lower-right side of the window. Doing so will close the installation window and open VirtualBox. Now that you've installed
and opened VirtualBox, you can create a virtual machine in order to run any operating system on your PC. 

video tutorial :- SOON TO COME 

## Mac OS
 
1.Open the VirtualBox website. Go to https://www.virtualbox.org/ in your Mac's Internet browser. This is the website from which you'll download the VirtualBox DMG file. 

2. Click Download VirtualBox. It's a blue button in the middle of the page. Doing so will open the downloads page. 

3. Click the OS X hosts link. You'll find this option in the middle of the downloads page. The VirtualBox DMG file will begin downloading onto your Mac. 

4. Open the "VirtualBox" DMG file. Once the VirtualBox DMG finishes downloading, double-click the file to open it. 

5.Double-click the "VirtualBox.pkg" icon. It's a brown box-shaped icon in the upper-left corner of the window. Doing so will prompt VirtualBox's installation window to open. 

6. Navigate through the installation prompts. Click Continue when prompted, then do the following:[1]

    Click Continue in the bottom-right corner of the window.
    Click Install in the bottom-right corner of the window.
    Enter your Mac user password when prompted.
    Click Install Software

7.Wait for the installation to complete. Once you're prompted to click Close in the bottom-right corner of the window, you've successfully installed VirtualBox on your Mac. 

8. Open VirtualBox. Click Spotlight Image titled Macspotlight.png, type in virtualbox, and double-click VirtualBox in the resulting drop-down menu. Now that
you've installed and opened VirtualBox, you can create a virtual machine in order to run any operating system on your Mac. 

video tutorial:- SOON TO COME 

## linux OS
1.  Open Terminal. This step will vary depending on your version of Linux, but you can usually open Terminal by selecting Image titled Macterminal.png
Terminal from the Menu. The Terminal window will pop up.

    You can also press Alt+Ctrl+T to open Terminal.


2.Enter the installation command. Type in sudo apt-get install virtualbox-qt and press Enter.

3.Type in the password that you use to log into your computer, then press Enter.

4. Confirm the installation by typing Y when prompted, then press Enter.

5. Wait for VirtualBox to finish installing. This will take a few minutes. When you see your computer account's username appear to the left of the command line, 
Terminal has successfully installed VirtualBox and is awaiting further commands. 

6.In terminal type in virtualbox and press Enter . This will prompt the VirtualBox main window to open. Now that you've installed and opened VirtualBox, you 
can proceed with creating a virtual machine in order to run any operating system on your computer.

video tutorial :- SOON TO COME 

## Creating A Virtual Machine 
Now that we have the virtualization host software installed, let’s start downloading some virtual machines. The first virtual machine we will install 
is Kali Linux. Kali Linux is one of the most popular hacking distributions used today and was created by Offensive Security. They provide .iso files that 
allow you to do a clean installation from burning the disk image to a CD or a bootable USB stick. However, there is a simpler option we are going to use with our 
virtual hosting software.

1. Visit https://www.offensive-security.com/kali-linux-vm-vmware-virtualbox-image-download/ There you can download the compressed VirtualBox files or the .ova files
for VirtualBox.
After the download completes, you will notice the file is a compressed .7z format. To unzip this file, you will need to install 7-zip. You can download the installation
file at https://7-zip.org. Just like the virtual machine file you will need to select the file based on the architecture you are using. And just like before, we will s
elect the 64-bit file you may choose depending on your system.

2.Next, wait for the file to be extracted. Once it’s done, move the folder to a location you are comfortable with and remember the location. Next, open VirtualBox and 
click File and then select “Open”.

3.Then, navigate to where your Kali Linux folder is located and click it. You will find the .vmx file. Click that and select “Open”. virtualbox will use the settings
in that file to create the virtual machine.

4.Click the Start icon to Start using Kali.

video tutorial :- SOON TO COME 



FOR any queries contact via mail on harmhacker@protonmail.com

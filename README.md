# tuneD-gui 
#### This is a GUI tool developed to utilize tunedD power daemon with a simple to use GUI for Ubuntu 24.04 and Fedora 40. Other distros will want to installed tuneD and use tuned-adm --help.

<br/>
<br/>

### Ubuntu 24.04 and Intel (AMD uses PPD defaults that is provided during the Ubuntu Install)

#### (Ubuntu with Intel Core Ultra Series 1) 

- Download, extract, browse into the directory, install deb by right clicking onto the deb package and installing with the Ubuntu app center. https://www.intel.com/content/www/us/en/download/819707/epp-tuning-package-for-linux-on-intel-core-ultra-mobile-processor.html

- Reboot

- Open a terminal, past in the following, press enter.

  ```
  sudo apt install curl -y && curl https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/Ultra-Series-1.sh | bash
  ```

- Reboot

<br/>
<br/>


#### (Ubuntu with Intel 11th, 12th and 13th Gen) 

- Open a terminal, past in the following, press enter.

  ```
  sudo apt install curl -y && curl https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/intel-13thGen.sh | bash
  ```

- Reboot

----------------------------------------

<br/>
<br/>

### Fedora 40 and Intel (AMD uses PPD defaults that is provided during the Fedora Install)


#### (Fedora with Intel Core Ultra Series 1) 

- Create a directory in your home directory called tuned-install.

- Install the GNOME Shell extension called AppIndicator/KStatusNotifierItem support using the Extension Manager. (If it's not installed, you can install it from the software store as Extension Manager)
  ![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/extension-manager.png)

- Download zipped folder https://www.intel.com/content/www/us/en/download/819707/epp-tuning-package-for-linux-on-intel-core-ultra-mobile-processor.html

- Open a terminal, past in the following, press enter.

  ```
  sudo dnf install curl -y && sudo apt install curl -y && curl https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/Ultra-Series-1-Fedora.sh | bash
  ```

- Reboot

<br/>
<br/>


#### (Fedora with Intel 11th, 12th and 13th Gen) 

- Open a terminal, past in the following, press enter.

  ```
  sudo dnf install curl -y && sudo apt install curl -y && curl https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/intel-13thGen-Fedora.sh | bash
  ```

- Reboot
  
--------------------------------------

<br/><br/>
![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/dark.png)

![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/light.png)
<br/><br/> 

## FAQ

- What does this thing do, though?  \
>Using tuneD (a system tuning daemon), users can select the power profile that best fits their individual needs.


- Do I need to disable PPD (Power Profile Daemon) for GNOME?  \
>Yes, both scripts do the heavy lifting for you - install, reboot and good to go.

- How do I use this?  \
>When installed and running on reboot, simply select the profile you wish to use.

![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/tuned-gui.gif)

- How do I know if this is working corrrectly?  \
>Run the following in a terminal, make sure it matches the profile you selected.

```
tuned-adm active
```
  
- What about dynamic tuning for tuneD?  \
>Coming soon.

- Why does this download the launcher graphic every time it runs?  \
>This was done during developement, it's going to be removed soon. But leave it as it's fine for now. This allows us to update the graphics remotely if needed. Besides, after it's installed, it will load the cached graphic if there is no internet acccess.

- What do I do with the Intel zipped folder?
>For the Fedora 40 installers, the zipped folder is handled for you so long as it is downloaded into the tuned-install directory that was suggested to be installed into your home direcctory previously.
>For Ubuntu 24.04 users, download it into home. Extract it. Browse inside of it, locate the deb package. Install the deb package. Follow the rest of the guide above.

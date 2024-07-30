# tuneD-gui For Ubuntu LTS 24.04

## Step 1 (Intel Core Ultra Series 1) 

- Download, extract, install deb. https://www.intel.com/content/www/us/en/download/819707/epp-tuning-package-for-linux-on-intel-core-ultra-mobile-processor.html

- Reboot

## Step 2 

- Open a terminal, past in the following, press enter.

  ```
  sudo apt install curl -y && curl https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/Ultra-Series-1.sh | bash
  ```

- Reboot

<br/>
<br/>

---------------------------------------

## Step 1 (Intel 11th, 12th and 13th Gen) 

- Open a terminal, past in the following, press enter.

  ```
  sudo apt install curl -y && https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/intel-13thGen.sh | bash
  ```

- Reboot


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

# tuneD-gui For Ubuntu LTS 24.04

## Step 1

- Download, extract, install deb. https://www.intel.com/content/www/us/en/download/819707/epp-tuning-package-for-linux-on-intel-core-ultra-mobile-processor.html

- Reboot

## Step 2

- Open a terminal, past in the following, press enter.

  ```
  sudo apt install curl -y && curl -sSL "https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/installer.sh" | bash
  ```

- Reboot

![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/dark.png)

![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/light.png)

<br/>
<br/>


## FAQ

- What does this thing do, though?  \
  *Using TuneD (a system tuning daemon), users can select the power profile that best fits their individual needs.*


- Do I need to disable PPD (Power Profile Daemon) for GNOME?  \
*Yes, instructions will be provided in the [Optimizing Ubuntu Battery Life](https://knowledgebase.frame.work/en_us/optimizing-ubuntu-battery-life-Sye_48Lg3) Knowledgebase article.*

- How do I use this?  \
*When installed and running on reboot, simply select the profile you wish to use.*  

![image](https://raw.githubusercontent.com/FrameworkComputer/tuned-gui/main/images/tuned-gui.gif)

- How do I know if this is working corrrectly?  \
*Run the following in a terminal, make sure it matctches the profile you selected.*

```
tuned-adm active
```
  
- What about dynamic tuning for tuneD?  \
*Coming soon.*

- Why does this download the launcher graphic every time it runs?  \
*This was done during developement, it's going to be removed soon. But leave it as is is fine.*

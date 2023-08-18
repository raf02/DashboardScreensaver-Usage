# Dashboard Screensaver

Dashboard Screensaver is an app that allows you to configure any web page - a dashboard, Home Assistant, Dakboard, or your favourite youtube video - as the screen saver for your Android TV. 

![enter image description here](https://play-lh.googleusercontent.com/j52mI4K3amG6oRc_Qug02apZu_TsTF0yrI2nb3HFSb6K5U_DollScNJLeLIp4ZrbpEo=w2560-h1440)

![enter image description here](https://play-lh.googleusercontent.com/qiJBuKE7hZMK-9_jz6qaLNqQdOrOO12sKHIkP7fHPcI4OmTtT0HaHqmPdRwyRb_OGA=w2560-h1440)

# Usage Instructions
For *most android TV devices* simply follow the instructions and **Open System Settings** to set 'Dashboard Screen Saver' as your default screen saver. Then set the **Dashboard URL** to the website you want to use as the screensaver. This works for most TV, nvidia shield and miboxes.
Note: this does not work for chromecast devices (eg. Google TV with chromecast), where the screensaver options have been locked down. chromecast devices require the adb method to change the screensaver

# Chromecast Devices - ADB Method
## 1. Enable Developer Options on the chromecast
First, go to **Settings > Device Preferences > About** then tap several times on the **Build** to unlock the Developer options.
![enter image description here](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2021/08/Android-tv-about-device.png?q=50&fit=crop&w=1500&dpr=1.5)
You will now be able to see the unlocked **Developer options** menu in the Device Preferences. Locate the **USB Debugging** toggle and enable it.
![enter image description here](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2021/08/Android-tv-enable-usb-debugging-developer-options.png?q=50&fit=crop&w=1500&dpr=1.5)On your Android TV, go to **Settings > Device Preferences > About > Status** and note down the **IP address**.
![enter image description here](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2021/08/Android-TV-status-ip-address.png?q=50&fit=crop&w=1500&dpr=1.5)
## 2. Install ADB Tools
Install ADB Tools on a PC. There's a few different tools that will allow you to do that - I use ['Minimal ADB'](https://androidfilehost.com/?fid=746010030569952951)
Alternative: Install ['Remote ADB Shell'](https://play.google.com/store/apps/details?id=com.cgutman.androidremotedebugger&hl=en_CA&gl=US) on an android phone. 

## 3. Change the screensaver using ADB commands
Enter `adb shell`
Enter ``settings put secure screensaver_components chyzinr.webpagescreensaver/.Screensaver``

## 4. Done!
When your screensaver kicks in, it should now start the website that you've configured.

# Linux iOS Utilities
I created these few simple shell scripts as a means of easily mounting and unmounting an unjailbroken iOS device, as Apple makes it very difficult to use most iOS devices with Linux unless you know what you are doing. You can easily choose which apps you want to mount by editing the imount script and commenting/uncommenting the apps you wish to mount. Some iOS apps which integrate wonderfully with Linux are [Local Storage](https://itunes.apple.com/app/id1339306324), a miniature, sandboxed file system for your phone;  [Edhita](https://itunes.apple.com/us/app/edhita-open-source-text-editor/id398896655), a dead simple text editor with the ability to view markdown and html files while you are editing them; [VLC](https://itunes.apple.com/app/apple-store/id650377962?pt=454758&ct=vodownloadpage&mt=8), a video player and media storage app; and [MuPDF](https://itunes.apple.com/us/app/mupdf/id482941798?mt=8), a versatile and lightweight pdf viewer, and the best thing about them is that they are all open source.

# Warning
I have had problems mounting more than 5 apps at any given time. In order to ensure that all the apps you want to mount will mount every time, I suggest that you only mount 5 or less apps at any given time. More than 5 apps may be possible, but I had not had much success. You can always jailbreak your iOS device to get around this limitation though, as ifuse and libimobiledevice allow you to mount the entire root filesystem for any jailbroken iOS device.

# Software Requirements
* [libimobiledevice](https://www.libimobiledevice.org/)

# Usage
First, clone this git repo by opening a terminal and typing ```git clone hts@ssh.gitgud.io:t/linux-ios-utils.git```

Then, enter the directory by typing ```cd linux-ios-utils```

If you want to mount your iOS device, first open the ```imount``` file in your favorite text editor and uncomment any of the apps you plan to mount. After you have done that, simply run the script by typing ```./imount```

The apps you chose will now be mounted to ```/mnt/ios```.

If you want to unmount your iOS device, such as when you want to unplug it from your computer, just type ```./iumount```

I have also included a script called ```irefresh```, which will kill and restart the usbmuxd daemon when the script is executed, which will start charging your phone if it is not charging when you plug it into your computer. 

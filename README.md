# Linux iOS Utilities
I created these few simple shell scripts as a means of easily mounting and unmounting an unjailbroken iOS device, as Apple makes it very difficult to use most iOS devices with Linux unless you know what you are doing. You can easily choose which apps you want to mount by editing the imount script and commenting/uncommenting the apps you wish to mount. Some iOS apps which integrate wonderfully which Linux are [Local Storage](https://itunes.apple.com/app/id1339306324), [Edhita](https://itunes.apple.com/us/app/edhita-open-source-text-editor/id398896655), [VLC](https://itunes.apple.com/app/apple-store/id650377962?pt=454758&ct=vodownloadpage&mt=8), and [MuPDF](https://itunes.apple.com/us/app/mupdf/id482941798?mt=8), and the best thing about them is that they are all open source.

# Warning
I have had problems mounting more than 4 apps at any given time. In order to ensure that all the apps you want to mount will mount every time, I suggest that you only mount 4 or less apps at any given time. More than 4 apps may be possible, but I had not had much success. You can always jailbreak your iOS device to get around this limitation though, as ifuse and libimobiledevice allow you to mount the entire root filesystem for any jailbroken iOS device.

# Software Requirements
* [libimobiledevice](https://www.libimobiledevice.org/)

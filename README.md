### Xdebug Setup Steps:

Xdebug Wizard URL: https://xdebug.org/wizard

1. Download xdebug file -> cut -> paste to xampp->php->ext

2. Copy the below code and paste under your php.ini file

```
xdebug.mode=debug
xdebug.start_with_request=trigger
xdebug.client_port=9003
xdebug.client_host = localhost
zend_extension="C:\xampp\php\ext\xdebug.dll"
```

3. Install PHP Debug extention your visual studio code.

*Always turn on your XAMPP
*You must put your file on XAMPP htdocs

[Edited]

> Error solved:
> [ PHP executable not found. Install PHP and add it to your PATH or set the php.executablePath setting ]

> You installed PHP IntelliSense extension, and this error because of it.
> <br> So if you want to fix this problem go to this menu:
> <br> File -> Preferences -> Settings
> <br> Then go here to find Settings.json file:

(https://ibb.co/XYBHzN7)

> Your XAMPP Folder must be in C Drive's root directory.

#### Add this code to your VS Code's settings.json File's bottom like this.

(https://ibb.co/HC9CSvx)

```
"php.debug.executablePath": "C:\\xampp\\php\\php.exe",
"php.validate.executablePath": "C:\\xampp\\php\\php.exe"
```

> Error solved:

#### PHP Xdebug Time-out Connecting to Debugging Client Error Solution Video Link:

https://youtu.be/cotcbEZkv7k

> [Xdebug: [Step Debug] Time-out connecting to debugging client, waited: 200 ms. Tried: localhost:9003 (through xdebug.client_host/xdebug.client_port).]

আরও একটি Error এর সমাধান এ্যাড করে দিলাম রিসোর্স ফাইলে। আপনারা কাইন্ডলি আমার দেয়া এই রিসোর্স থেকে php(.ini) ফাইলের জন্য যেই কোড দিয়েছি, সেটা কপি করে আনার পর, (.dll) ফাইলের পাথ ভিডিওতে যেভাবে দেখানো হয়েছে , সেই ভাবেই পাথ কপি করে এনে php(.ini) ফাইলে পেস্ট করবেন।

# Creating your own custom theme for Snowboard or Anemone
### Contents
* [Getting Started](#Getting-Started)
* Theme Configuration
* Creating Icons
* Exporting Icons
* Icon Masks
* Packaging

## Getting Started

**Note: Without the proper folder structure, your theme may not show up!**

* Create a new folder called `themeName.theme` (Replace themeName with your desired theme name)
* Within `themeName.theme` folder, create another folder called `IconBundles` (**You cannot change this name**)

## Theme Configuration

* Now, inside the `themeName.theme` folder, create a file called `Info.plist` and paste the following
```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
  <plist version="1.0">
  <dict>
    <key>PackageName</key>
    <string>ThemeName</string>
    <key>ThemeType</key>
    <string>Icons</string>
  </dict>
</plist>
```
* Replace `PackageName` with the name of the Pacakge and replace `ThemeName` with the Theme Name

Now, you might ask what is the difference between `PackageName` and `ThemeName`?

Well, if for example you want to publish two variants of your icons, one dark and one white but you do not want the user to seperately install them.
Then, you would name the package `MyTheme` and include two themes `Blackie` and `White` thus creating two entries. More about this in the end

## Creating Icons

* Open up the Image Editor of your choice and create a new file having a resolution of 512x512 

**Note: Due to IconBundles, we just need to create the icons in one size and they get resized automaticaly** :ghost:

**Want to create rounded icons?**
Create them squared only, we will learn how to apply masks!

## Exporting Icons
**Note: All icons must be saved as `*.png` (Tip: This means you can even create partially transparent icons!)**

* All Icons must be saved in themeName>IconBundles as `bundleID-large.png`

##### Finding BundleIDs

**Stock Application BundleIDs**
| Name        | BundleID             |
|-------------|----------------------|
| App Store   | com.apple.AppStore   |
| Apple Watch | com.apple.Bridge     |
| Calculator  | com.apple.calculator |
| Calendar | com.apple.mobilecal |
| Camera | com.apple.camera |
| Classroom | com.apple.classroom |
| Clock | com.apple.mobiletimer |
| Compass | com.apple.compass |
| FaceTime | com.apple.facetime |
| Files | com.apple.DocumentsApp |
| Game Center | com.apple.gamecenter |
| Health | com.apple.Health |
| Home | com.apple.Home |
| iBooks | com.apple.iBooks |
| iTunes Store | com.apple.MobileStore | 
| Mail | com.apple.mobilemail |
| Maps | com.apple.Maps |
| Measure | com.apple.measure |
| Messages | com.apple.MobileSMS |
| Music | com.apple.Music |
| News | com.apple.news |
| Notes | com.apple.mobilenotes |
| Phone | com.apple.mobilephone |

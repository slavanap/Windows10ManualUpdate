[![Build status](https://ci.appveyor.com/api/projects/status/c86j63q3hm64fb46?svg=true)](https://ci.appveyor.com/project/slavanap/windows10manualupdate)

# Install Windows Updates in Windows 10 manually

Note, this method *may not work* properly in Windows 10 Home.

Before running this app you must turn off automatic updates installation. This could be done via *Group Policy Object Editor* MMC snap-in or via importing registry files into Windows Registry.

In order to do it via MMC:

* Press Win+R. Type `mmc.exe`. Hit Enter.
* Navigate menu *File -> Add/Remove Snap-in*. Select *Group Policy Object Editor*, click *Add* to add it to the list on the right. Click *Finish*, then *OK*.
* On the left navigate to *Local Computer Policy -> Computer Configuration -> Administrative Templates -> Windows Components -> Windows Update*. Select that folder.
* In the list select *Configure Automatic Updates* policy and set it to *Disabled*. This setting will disable automatic updates check and installation, but if you navigate to Updates in Windows Setting you'll implicitly launch automatic updates check and installation.
* Change other options in MMC, if you really know what you're doing.

Another approach is to use Registry files:

* [manual updates policy.reg](../master/manual%20updates%20policy.reg)
* [manual updates & no restarts policies.reg](../master/manual%20updates%20&amp;%20no%20restarts%20policies.reg)

Be sure you know how to backup registry and undo changes that are declared in these files. These files are like 10 lines long: don't hesitate to read them!

![App User Interface](https://github.com/slavanap/Windows10ManualUpdate/blob/master/app_ui.gif?raw=true)

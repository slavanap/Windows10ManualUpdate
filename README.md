#Install Windows Updates in Windows 10 manually

Note, this method may not work properly in Windows 10 Home.

Before running this app you must to turn off automatic updates installation. This could be done via *Group Policy Object Editor* MMC snap-in or via importing registry files into Windows Registry, pick up the right file for you among `.reg` files in the repository root.

[manual updates policy.reg](https://github.com/slavanap/Windows10ManualUpdate/tree/master/manual updates policy.reg)

[manual updates & no restarts policies.reg](https://github.com/slavanap/Windows10ManualUpdate/tree/master/manual updates & no restarts policies.reg)

Be sure you know how to backup registry and undo changes that are declared in these files. These files are like 10 lines long: don't hesitate to read them.

![App User Interface](https://github.com/slavanap/Windows10ManualUpdate/blob/master/app_ui.gif?raw=true)

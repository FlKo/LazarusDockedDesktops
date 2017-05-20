## Lazarus...*Docked*...Desktops

#### Desktop configuration files for Lazarus IDE that try to resemble the 'Look'n'Feel' of Embarcadero™ RAD Studio™.
---

For all those who ever wanted "their" Lazarus to look and behave close to the latest releases of Delphi™ / C++ Builder™
but gave up because of some very annoying bugs, here comes a solution: 

**Preconfigured Desktop Files: The Lazarus...*Docked*...Desktops.**

---

Get the [latest release here](https://github.com/FlKo/LazarusDockedDesktops/releases/latest).

---

- [May 2017 Update: LDDs are compatible with Lazarus 1.9.0 trunk](#may-2017-update-ldds-are-compatible-with-lazarus-1.9.0-trunk)
- [ToolButton *Run without Debugging*](#toolbutton-run-without-debugging)
- [Structural highlighting](#structural-highlighting)
- [November 2016 Update: New StudioPlus Desktops](#november-2016-update-new-studioplus-desktops)
- [How to install](#how-to-install)
---

## May 2017 Update: **LDD**s are compatible with Lazarus 1.9.0 trunk 

Keep in mind: Lazarus...*Docked*...Desktops are compatible even with development versions of Lazarus and have been tested with **Lazarus 1.9.0** / **FPC 3.1.1 trunk** .

The recommended installation method for latest trunk versions is via the excellent [fpcupdeluxe](https://github.com/newpascal/fpcupdeluxe) tool. 

Albeit those versions may be not as stable as the *official* ones, you have may some very neat features that are not available in the *stable* builds.

Here is a picture of a recent *trunk* version of Lazarus 1.9.0 with *LDD*s applied:

![ide](https://cloud.githubusercontent.com/assets/22365547/26276002/13d460dc-3d6e-11e7-86b2-296fbce97f8b.PNG)
The instructions below may require a recent *trunk* version of Lazarus.

### ToolButton *Run without Debugging*

As you can see, there's an additional **Run without Debugging** button next to the **Run** button in the IDE CoolBar.

You can get this in the *IDE options* by selecting

- *Environment* -> *IDE CoolBar* -> Select the right part of the tool bar under *Add/Config/Delete Toolbar(s)* and then click *Configure*.

![c_a](https://cloud.githubusercontent.com/assets/22365547/26275942/c1fd3848-3d6c-11e7-8f9d-48b6d4b7f9d0.PNG)

- Now open the node *Run menu commands* and select *Run without Debugging (Shift+Ctrl+F9)*
- Click the *right arrow* button highlighted yellow in the following picture

![c_a1](https://cloud.githubusercontent.com/assets/22365547/26275943/c20019fa-3d6c-11e7-8c46-6d8a5aab7035.PNG)

- Now select the added command and then click the *up arrow* button highted in the picture below *6x*, so the *Run without Debugging* command is placed straight above the *Run (F9)* command.
- Click *OK*, then click *OK* again, to close the *IDE options* window.

You now have the option to run your code without invoking the debugger like in Delphi.

![c_a2](https://cloud.githubusercontent.com/assets/22365547/26275944/c206145e-3d6c-11e7-97f1-8697be510b5f.PNG)

### Structural highlighting

You can now also have **structural highlighting** of your code, as it is available in Delphi by default since **XE8** (or earlier via the *Castalia* plugin). For more infos about structural highlighting in Lazarus take a look [here](http://forum.lazarus-ide.org/index.php/topic,30122.0.html?PHPSESSID=eovlh2rh5jinlilruh1h4l3fm5).

To enable it, open the *IDE options* and check

- *Editor* -> *Display* -> *Markup and Matches* -> *Matching Keywords* -> *Outline (global)*.

![c_a3](https://cloud.githubusercontent.com/assets/22365547/26275945/c206960e-3d6c-11e7-9821-6278859a0793.PNG)

---

## November 2016 Update: New **StudioPlus** Desktops

Download the new [StudioPlusComplete](https://github.com/FlKo/LazarusDockedDesktops/releases/latest) desktop, which is better devised and will be frequently improved.

- Improved button layout in editor toolbar
- Message window can be shrinked and maximized comfortably by sliding up/down with the mouse
- Event Log, Call stack, BreakPoints, Threads, Assembler and Debug Output are now **all** selectable via tabs in Debug Desktop

---

![c1](https://cloud.githubusercontent.com/assets/22365547/20536007/9b11ada2-b0e7-11e6-88ca-a604972f1bc8.PNG)
![c2](https://cloud.githubusercontent.com/assets/22365547/20536014/9fc2651c-b0e7-11e6-8141-9b0650fb4a68.PNG)

---

## How to install

So what do we need?
- A computer ;-)
- A running copy of *Windows™*, *Mac OS X™* or *Linux*.
- An installation of [Lazarus](http://www.lazarus-ide.org) (preferably version 1.6 or newer).
- The installation of the packages **AnchorDockingDsgn** and **sparta_DockedFormEditor** which are already included in Lazarus.
- The import of one or more of the **Lazarus...*Docked*...Desktops** from this repository.

---

#### Step 1: Installation of the *AnchorDockingDsgn* package

Open Lazarus and click on *Install/Uninstall Packages* in the *Packages* menu.

![01_install](https://cloud.githubusercontent.com/assets/22365547/18887723/98669c2a-84f5-11e6-9e2b-dbc4ed248730.png)

Now select *anchordockingdsgn x.x* (where *x.x* the version number) in the ListView on the right side and click on *Install selection*.
Finally click on *Save and rebuild IDE*.

![02_install](https://cloud.githubusercontent.com/assets/22365547/18887724/986c8194-84f5-11e6-8e5b-3d6e70d9d6f8.png)

Confirm the new package set in the next dialog with *Continue*.

![03_install](https://cloud.githubusercontent.com/assets/22365547/18887726/98718c16-84f5-11e6-83cb-60a02ed6782f.png)

Now wait for the IDE to re-compile and restart. This may take some time so be patient.

---

#### Step 2: Installation of the *sparta_DockedFormEditor* package

It is time to install the second package. You can try it in the same way as described in step 1, if the component *sparta_dockedformeditor* is being listed in the ListView. If not, click on *Open Package File (.lpk) ...* in the *Package* menu.

![04_install](https://cloud.githubusercontent.com/assets/22365547/18887725/986ff734-84f5-11e6-88e1-449e9a975037.png)

Browse to */components/sparta/dockedformeditor/* within your Lazarus home directory and open *sparta_dockedformeditor.lpk*.

![05_install](https://cloud.githubusercontent.com/assets/22365547/18887727/9872b2da-84f5-11e6-840a-1f680303f874.png)

In the following dialog, click on *Use >>* and then *Install*.

![06_install](https://cloud.githubusercontent.com/assets/22365547/18887728/987ab9c6-84f5-11e6-97df-42e81f0350b6.png)

Confirm the *Rebuild Lazarus?* dialog and wait a second time for the IDE to re-compile and restart. This may again take some moments.

![07_install](https://cloud.githubusercontent.com/assets/22365547/18887729/987e269c-84f5-11e6-814d-70dd6f7b5db3.png)

---

#### Step 3: Importing the *Lazarus...Docked...Desktops*

After the restart of the IDE it looks...hmm...scary. But we will now fix that. You can try to rearrange the windows for yourself as you like, but be prepared for some unlovely bugs.
It's better to load the prepared laylouts.

Select *Desktops* in the *Tools* menu.

![08_install](https://cloud.githubusercontent.com/assets/22365547/18887731/988647e6-84f5-11e6-9ee4-dc2c0719a751.png)

Now you're in the *Manage desktops* dialog. First, uncheck the option *Auto save active desktop*, then click *Import*.

![09_install](https://cloud.githubusercontent.com/assets/22365547/18887732/988938ac-84f5-11e6-9a9e-c5e2c4e6bb30.png)

Browse to the folder in which the clone of this repository resides and open one of the *XML* files. I recommend *StudioPlusComplete.xml* in *StudioPlus* folder because it includes both the *default* and the *debug* desktop and is the desktop which will get updates frequently.

![10_install](https://cloud.githubusercontent.com/assets/22365547/18887733/988dfda6-84f5-11e6-86b2-069e2131d65e.png)

Confirm the next *Desktop name* dialog with OK.

![11_install](https://cloud.githubusercontent.com/assets/22365547/18887734/988ff534-84f5-11e6-8ef7-345fd59d2f7e.png)

![12_install](https://cloud.githubusercontent.com/assets/22365547/18887735/98951d84-84f5-11e6-906d-1a57ac418dc5.png)

After that, select the desktop *debug docked* and click on the green bug symbol on the right to toggle it as the debug desktop. Finally, close *Manage desktops*.

Now it is important that you **restart the IDE** manually to complete the procedure (sometimes it seems to be necessary to restart Lazarus **twice**).

---

#### Step 4: Colors and Editor Font

To have a more 'modern' look, apply these changes to the IDE options (*Tools->Options* or *Shift+Ctrl+O*)

- *Display* -> *Default editor font* := *Consolas* (if you are on Windows™); Editor font size := 10.
- You can move the right gutter to *120*, but that's my personal preference.

![14_install](https://cloud.githubusercontent.com/assets/22365547/18889777/bdfa47da-84fe-11e6-9e16-1b4a13a2852c.png)

- *Display* -> *Colors* -> Select *Delphi* theme.

![13_install](https://cloud.githubusercontent.com/assets/22365547/18889778/bdfaabc6-84fe-11e6-83ba-fc7951c66f5d.png)

- *Environment* -> *Object Inspector* -> Select *Use default Delphi settings* and then set the checkboxes as shown.

![15_install](https://cloud.githubusercontent.com/assets/22365547/18916865/2a1bf6f6-8596-11e6-9aeb-db4d41f89e8d.png)

- *Environment* -> *Messages Window* -> Click on *Pastel Colors*.

![19_install](https://cloud.githubusercontent.com/assets/22365547/19022722/e506f966-88de-11e6-8b65-fb443383369c.png)

If you like to have Lazarus to automatically remove empty methods like the default behaviour of RAD Studio, you must check

- *Editor* -> *Completion and Hints* -> *Auto remove empty methods*.

![23_install](https://cloud.githubusercontent.com/assets/22365547/19165167/1a275d58-8c03-11e6-862a-03c6f35fa794.png)

---

#### Step 5: More personal preferences

The next things are my personal settings and may not be everyone's favourite. So feel free to use it.

A very annoying thing in RAD Studio is the impossibility to prevent the cursor from moving beyond the end of the line.
In Larazus, its just an unchecking of the *Editor* -> *General* - *Caret past end of line* checkbox.

![20_install](https://cloud.githubusercontent.com/assets/22365547/19088442/6d3b0b36-8a76-11e6-9ad4-d3b081d58c66.png)

I like a little more 'horizontal space' in my code. Pascal is a little bit too 'compact' for me (coming from a C++ background).
I checked *Insert space in front of Symbol* and *Insert space after Symbol* in *Editor* -> *Codetools* -> *Space* for that reason.

![21_install](https://cloud.githubusercontent.com/assets/22365547/19165164/14462dec-8c03-11e6-8cba-84b053c3a370.png)

Below are some more settings I like:

![22_install](https://cloud.githubusercontent.com/assets/22365547/19165166/16e3ba38-8c03-11e6-8013-68186753de38.png)
![24_install](https://cloud.githubusercontent.com/assets/22365547/19165169/1d0524ba-8c03-11e6-8f9a-32aaf92738b7.png)
![25_install](https://cloud.githubusercontent.com/assets/22365547/19166981/188ded20-8c0a-11e6-9163-1b08e4ba69bb.png)

---

Before you now finally start, don't forget to take a look at these "incredible" screenshots below:

##### The Embedded Form Editor

![Image of Studio Desktop - Default Form Editor](https://cloud.githubusercontent.com/assets/22365547/18885386/c3408c44-84eb-11e6-9b3a-6c8790790827.gif)

##### The Code Editor

![Image of Studio Desktop - Default Code Editor](https://cloud.githubusercontent.com/assets/22365547/18885388/c3488ee4-84eb-11e6-9f6c-4fda8fdf53cb.GIF)

##### The Debug Desktop

![Image of Studio Desktop - Default Debug](https://cloud.githubusercontent.com/assets/22365547/18885387/c343c986-84eb-11e6-8059-2304e5b4f9b2.GIF)


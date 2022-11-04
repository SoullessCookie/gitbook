# Exercise 2 - Perform a Clean Install

### **Exercise 2 - Perform a Clean Install** <a href="#cn-m1-93" id="cn-m1-93"></a>

An operating system can be installed using multiple methods. Some of these methods are listed below:

* Unattended installation
* In-place upgrade
* Clean install
* Repair installation
* Multiboot
* Remote network installation
* Image deployment
* Recovery partition
* Restore/Refresh

For all the methods listed above, the actual process of installation remains the same. Only the choice of boot device differs.



#### **Task 1 - Installing an Operating System** <a href="#cn-m1-115" id="cn-m1-115"></a>

A clean install is a fresh install. To do this, perform the following steps:

_**Step 1**_

Ensure you are connected to **PLABWIN10** and **Hyper-V Manager** window is open.

Right-click **PLABWIN101**, and then select **Start**. This will power on the device.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-10.jpg?v=18" alt="Figure 2.1 Screenshot of PLABWIN10: Right-clicking the virtual machine and selecting Start."><figcaption><p>Figure 2.1 Screenshot of PLABWIN10: Right-clicking the virtual machine and selecting Start.</p></figcaption></figure>

_**Step 2**_

Right-click **PLABWIN101**, then select **Connect**.

Alternatively, you can double-click the black icon inside the **PLABWIN101** section that contains **Hyper-V** text.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-11.jpg?v=18" alt="Figure 2.2 Screenshot of PLABWIN10: Double-clicking the black colored icon to enlarge the virtual machine."><figcaption><p>Figure 2.2 Screenshot of PLABWIN10: Double-clicking the black colored icon to enlarge the virtual machine.</p></figcaption></figure>

_**Step 3**_

If the virtual machine window is not properly visible, click **Maximize**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-12.jpg?v=18" alt="Figure 2.3 Screenshot of PLABWIN10: Maximizing the virtual machine window."><figcaption><p>Figure 2.3 Screenshot of PLABWIN10: Maximizing the virtual machine window.</p></figcaption></figure>

_**Step 4**_

The process of installation starts and the **Windows Setup** dialog box is displayed.

Keep the default values and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-13.jpg?v=18" alt="Figure 2.4 Screenshot of PLABWIN10: Displaying the dialog box for acquiring language, time, date, and keyboard or input related method-related information."><figcaption><p>Figure 2.4 Screenshot of PLABWIN10: Displaying the dialog box for acquiring language, time, date, and keyboard or input related method-related information.</p></figcaption></figure>

_**Step 5**_

Click **Install now**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-14.jpg?v=18" alt="Figure 2.5 Screenshot of PLABWIN10: Clicking the Install now button."><figcaption><p>Figure 2.5 Screenshot of PLABWIN10: Clicking the Install now button.</p></figcaption></figure>

_**Step 6**_

The **Setup is starting** window appears. You will be moved to the next screen automatically after a few seconds.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-15.jpg?v=18" alt="Figure 2.6 Screenshot of PLABWIN10: Displaying the Setup is starting screen."><figcaption><p>Figure 2.6 Screenshot of PLABWIN10: Displaying the Setup is starting screen.</p></figcaption></figure>

_**Step 7**_

Wait till the **Select the operating system you want to install** panel appears.

Keep the default selection and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-16.jpg?v=18" alt="Figure 2.7 Screenshot of PLABWIN10: Selecting the Windows 10 version to install."><figcaption><p>Figure 2.7 Screenshot of PLABWIN10: Selecting the Windows 10 version to install.</p></figcaption></figure>

_**Step 8**_

Tick the **Accept the license terms** checkbox and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-17.jpg?v=18" alt="Figure 2.8 Screenshot of PLABWIN10: Accepting the license terms."><figcaption><p>Figure 2.8 Screenshot of PLABWIN10: Accepting the license terms.</p></figcaption></figure>

_**Step 9**_

There are two options for this window:

* **Upgrade**: This option keeps all the files, setting and applications intact. These are moved to the newly installed operating system. If the data in the previous setup is required, then this option should be used.
* **Custom**: This is also known as a clean installation. In this type of installation, the data present in the previous operating system is erased. Files should be backed-up before proceeding with this type of installation.

Select **Custom: Install Windows only (advanced**).

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-18.jpg?v=18" alt="Figure 2.9 Screenshot of PLABWIN10: Choosing the Custom installation."><figcaption><p>Figure 2.9 Screenshot of PLABWIN10: Choosing the Custom installation.</p></figcaption></figure>

_**Step 10**_

Click the **New** link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-19.jpg?v=18" alt="Figure 2.10 Screenshot of PLABWIN10: Clicking the New link to create a new partition."><figcaption><p>Figure 2.10 Screenshot of PLABWIN10: Clicking the New link to create a new partition.</p></figcaption></figure>

_**Step 11**_

You need to define the partition size. In the **Size** text box, change to the following value:

```
50000
```

Click **Apply**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-20.jpg?v=18" alt="Figure 2.11 Screenshot of PLABWIN10: Setting the size of the partition."><figcaption><p>Figure 2.11 Screenshot of PLABWIN10: Setting the size of the partition.</p></figcaption></figure>

_**Step 12**_

The **Windows Setup** dialog box is displayed. Click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-21.jpg?v=18" alt="Figure 2.12 Screenshot of PLABWIN10: Displaying the Windows Setup dialog box with the message about creating additional partitions."><figcaption><p>Figure 2.12 Screenshot of PLABWIN10: Displaying the Windows Setup dialog box with the message about creating additional partitions.</p></figcaption></figure>

_**Step 13**_

Select **Drive 0 Unallocated space** and click the **New** link again.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-22.jpg?v=18" alt="Figure 2.13 Screenshot of PLABWIN10: Showing a newly created partition and then selecting the leftover space and clicking the New link."><figcaption><p>Figure 2.13 Screenshot of PLABWIN10: Showing a newly created partition and then selecting the leftover space and clicking the New link.</p></figcaption></figure>

_**Step 14**_

Accept the default value mentioned in the **Size** text box. Click **Apply**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-23.jpg?v=18" alt="Figure 2.14 Screenshot of PLABWIN10: Setting the default size and clicking Apply."><figcaption><p>Figure 2.14 Screenshot of PLABWIN10: Setting the default size and clicking Apply.</p></figcaption></figure>

_**Step 15**_

Notice that two partitions are now created. The third partition is reserved for the system. Select **Disk 0 Partition 2** and then click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-24.jpg?v=18" alt="Figure 2.15 Screenshot of PLABWIN10: Selecting the partition for installation."><figcaption><p>Figure 2.15 Screenshot of PLABWIN10: Selecting the partition for installation.</p></figcaption></figure>

_**Step 16**_

The **Installing Windows** dialog box is displayed when the installation procedure begins.

Wait for the procedure to be completed. The virtual machine may restart multiple times during the course of this procedure.

_**Note:** This installation takes about 20-30 minutes to complete._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-25.jpg?v=18" alt="Figure 2.16 Screenshot of PLABWIN10: Showing the installation progress on the Installing Windows screen."><figcaption><p>Figure 2.16 Screenshot of PLABWIN10: Showing the installation progress on the Installing Windows screen.</p></figcaption></figure>

_**Step 17**_

The installation will continue.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-26.jpg?v=18" alt="Figure 2.17 Screenshot of PLABWIN10: Showing the installation progress on the Installing Windows screen."><figcaption><p>Figure 2.17 Screenshot of PLABWIN10: Showing the installation progress on the Installing Windows screen.</p></figcaption></figure>

_**Step 18**_

Finally, you need to restart Windows. Click **Restart now**.

_**Note:** If you do not restart window within 15 seconds, it will auto restart._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-27.jpg?v=18" alt="Figure 2.18 Screenshot of PLABWIN10: Clicking the Restart now button."><figcaption><p>Figure 2.18 Screenshot of PLABWIN10: Clicking the Restart now button.</p></figcaption></figure>

_**Step 19**_

Windows will boot. You will be prompted to press a key to boot from CD.

Remember that you have already loaded Windows. **Do NOT press any key.** If you press a key at this point, the installation will restart.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-28.jpg?v=18" alt="Figure 2.19 Screenshot of PLABWIN10: Showing the boot from CD screen."><figcaption><p>Figure 2.19 Screenshot of PLABWIN10: Showing the boot from CD screen.</p></figcaption></figure>

_**Step 20**_

Windows Setup is now configuring Windows services.

**This will take a few minutes to complete.** You will be taken to a few more screens.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-29.jpg?v=18" alt="Figure 2.20 Screenshot of PLABWIN10: Showing the newly installed Windows configuration."><figcaption><p>Figure 2.20 Screenshot of PLABWIN10: Showing the newly installed Windows configuration.</p></figcaption></figure>

_**Step 21**_

Windows will reboot to finalize the setup. Notice that the virtual machine is now closed.

On the **Virtual Machine Connection** dialog box, click **Reconnect**.

_**Note**: If the **Virtual Machine Connection** dialog box doesn’t appear, please proceed to **Step 24**._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-30.jpg?v=18" alt="Figure 2.21 Screenshot of PLABWIN10: Reconnecting with the virtual machine."><figcaption><p>Figure 2.21 Screenshot of PLABWIN10: Reconnecting with the virtual machine.</p></figcaption></figure>

_**Step 22**_

Maximize the **PLABWIN101 on PLABWIN10 - Virtual Machine Connection** dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-31.jpg?v=18" alt="Figure 2.22 Screenshot of PLABWIN10: Maximizing the virtual machine window size."><figcaption><p>Figure 2.22 Screenshot of PLABWIN10: Maximizing the virtual machine window size.</p></figcaption></figure>

_**Step 23**_

The **Just a moment** screen is displayed. This will stay for a few minutes.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-32.jpg?v=18" alt="Figure 2.23 Screenshot of PLABWIN10: Showing the Just a moment screen."><figcaption><p>Figure 2.23 Screenshot of PLABWIN10: Showing the Just a moment screen.</p></figcaption></figure>

_**Step 24**_

On the **Let’s start with region. Is this right?** screen, select **United Kingdom** and then click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-33.jpg?v=18" alt="Figure 2.24 Screenshot of PLABWIN10: Selecting a region for this installation."><figcaption><p>Figure 2.24 Screenshot of PLABWIN10: Selecting a region for this installation.</p></figcaption></figure>

_**Step 25**_

On the **Is this the right keyboard layout?** screen, select **United Kingdom** as the keyboard layout and then click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-34.jpg?v=18" alt="Figure 2.25 Screenshot of PLABWIN10: Selecting a keyboard layout for this installation."><figcaption><p>Figure 2.25 Screenshot of PLABWIN10: Selecting a keyboard layout for this installation.</p></figcaption></figure>

_**Step 26**_

On the **Want to add a second keyboard layout?** screen, click **Skip**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-35.jpg?v=18" alt="Figure 2.26 Screenshot of PLABWIN10: Skipping adding a secondary keyboard."><figcaption><p>Figure 2.26 Screenshot of PLABWIN10: Skipping adding a secondary keyboard.</p></figcaption></figure>

_**Step 27**_

On the **Let’s connect you to a network** screen, click the **Skip for Now** link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-36.jpg?v=18" alt="Figure 2.27 Screenshot of PLABWIN10: Clicking the Skip for now link for the Ethernet network."><figcaption><p>Figure 2.27 Screenshot of PLABWIN10: Clicking the Skip for now link for the Ethernet network.</p></figcaption></figure>

_**Step 28**_

On the **Who’s going to use this PC?** screen, type the following inside the text box:

```
PLABUser
```

Then, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-37.jpg?v=18" alt="Figure 2.28 Screenshot of PLABWIN10: Creating a user account who will use this installation."><figcaption><p>Figure 2.28 Screenshot of PLABWIN10: Creating a user account who will use this installation.</p></figcaption></figure>

_**Step 29**_

On the **Create a super memorable password** screen, type the following text in the field password field:

Passw0rd

Then, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-38.jpg?v=18" alt="Figure 2.29 Screenshot of PLABWIN10: Entering a password during the windows 10 installation process."><figcaption><p>Figure 2.29 Screenshot of PLABWIN10: Entering a password during the windows 10 installation process.</p></figcaption></figure>

_**Step 30**_

On the **Confirm your password** screen, re-enter the password in the text field:

Passw0rd

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-39.jpg?v=18" alt="Figure 2.30 Screenshot of PLABWIN10: Confirming the password for the user."><figcaption><p>Figure 2.30 Screenshot of PLABWIN10: Confirming the password for the user.</p></figcaption></figure>

_**Step 31**_

On the **Add a hint for your password** screen, type the following in the text field:

```
default password
```

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-40.jpg?v=18" alt="Figure 2.31 Screenshot of PLABWIN10: Setting a hint for the password."><figcaption><p>Figure 2.31 Screenshot of PLABWIN10: Setting a hint for the password.</p></figcaption></figure>

_**Step 32**_

On the **Make Cortana your personal assistant?** screen, click **No**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-41.jpg?v=18" alt="Figure 2.32 Screenshot of PLABWIN10: Clicking No for the Cortana integration."><figcaption><p>Figure 2.32 Screenshot of PLABWIN10: Clicking No for the Cortana integration.</p></figcaption></figure>

_**Step 33**_

On the **Choose privacy settings for your device** screen, click **Accept**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-42.jpg?v=18" alt="Figure 2.33 Screenshot of PLABWIN10: Accepting the privacy settings."><figcaption><p>Figure 2.33 Screenshot of PLABWIN10: Accepting the privacy settings.</p></figcaption></figure>

_**Step 34**_

The settings configured in the previous steps will be applied. Wait until the process is completed. This may take a few minutes.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-43.jpg?v=18" alt="Figure 2.34 Screenshot of PLABWIN10: Finalizing the Windows installation."><figcaption><p>Figure 2.34 Screenshot of PLABWIN10: Finalizing the Windows installation.</p></figcaption></figure>

_**Step 35**_

When the installation process is completed, the desktop of the newly installed operating system will appear.

Let the virtual machine reach this stage, and then close the virtual machine window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-44.jpg?v=18" alt="Figure 2.35 Screenshot of PLABWIN10: Showing the desktop after to completion of windows 10 installation."><figcaption><p>Figure 2.35 Screenshot of PLABWIN10: Showing the desktop after to completion of windows 10 installation.</p></figcaption></figure>

_**Note:** If you need to create a multiboot system, restart your system and then choose to boot from the DVD. After which, you can follow the following steps:_\
_1. Follow step 1 to step 4 of this exercise._\
_2. Then, follow step 10 to step 13 of this exercise._\
_3. Once the steps are followed, then The **Where do you want to install the window?** panel appears._\
_4. Select **Drive 0 Partition 3** and continue with the installation._\
_5. Follow step 21 to 32 of this exercise to complete the procedure._\
_6. After the virtual machine restarts when installation is completed, you will get two options to choose from._\
_There are no hard and fast rules of which two operating systems you want to boot from. Remember that if you were multibooting with Linux, the default operating system would be Linux. The system will directly boot from Linux unless you change it to Windows manually._

_**Step 36**_

**Close** all open windows.

#### **Task 2 - Create a Recovery Partition** <a href="#cn-m1-311" id="cn-m1-311"></a>

The recovery partition is a part of a disk drive which is created to hold an image of the system taken at a particular point of time. Creating a recovery partition helps in recovering data if it is lost.

Recovery partition’s files are used for reinstalling operating system back on the machine. Windows operating system has inbuilt functionality to create a recovery partition.

Below is the demonstration of how to create a recovery partition.

**Alert**: This task **cannot** be performed in the lab environment as it requires an external drive. Below is a demonstration of how you would perform these steps.

_**Step 1**_

Search for the following in the search bar:

```
Create a recovery drive
```

Select **Create a recovery drive** from the search results.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-45.jpg?v=18" alt="Figure 2.36: Selecting Create a recovery drive from the search results."><figcaption><p>Figure 2.36: Selecting Create a recovery drive from the search results.</p></figcaption></figure>

_**Step 2**_

The **Recovery Drive** wizard is displayed. Keep the default selection and click **Next**.

_**Note:** If prompted with **User Account Control** dialog box, click **Yes**._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-46.jpg?v=18" alt="Figure 2.37: Clicking Next on the Create a recovery drive page."><figcaption><p>Figure 2.37: Clicking Next on the Create a recovery drive page.</p></figcaption></figure>

_**Step 3**_

The process of creating a recovery partition starts.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-47.jpg?v=18" alt="Figure 2.38: Showing the initial phase of recovery partition creation process."><figcaption><p>Figure 2.38: Showing the initial phase of recovery partition creation process.</p></figcaption></figure>

_**Step 4**_

A message about the recovery drive size requirement is shown. Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-48.jpg?v=18" alt="Figure 2.39: Screen shows a screen of selection of a device for creating the recovery partition"><figcaption><p>Figure 2.39: Screen shows a screen of selection of a device for creating the recovery partition</p></figcaption></figure>

_**Step 5**_

Click **Create**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-49.jpg?v=18" alt="Figure 2.40: Showing a warning message about losing data."><figcaption><p>Figure 2.40: Showing a warning message about losing data.</p></figcaption></figure>

_**Step 6**_

The process of creating a recovery drive starts. It will take a few minutes to complete.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-50.jpg?v=18" alt="Figure 2.41: Formatting the drive for the recovery partition."><figcaption><p>Figure 2.41: Formatting the drive for the recovery partition.</p></figcaption></figure>

_**Step 7**_

Once the recovery drive is created, it is visible inside the **This PC** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-51.jpg?v=18" alt="Figure 2.42: Showing a newly created recovery partition."><figcaption><p>Figure 2.42: Showing a newly created recovery partition.</p></figcaption></figure>

**Alert**: The next task **can** be performed in the lab environment.

#### **Task 3 - Prepare for an Unattended Installation** <a href="#cn-m1-350" id="cn-m1-350"></a>

Assume that you have to install Windows 10 on multiple systems at the same time. You can perform an unattended installation on all these systems at one go.

This is done with the help of Autounattended.xml, which needs to be copied to the root of the USB or DVD drive.

A sample of this file can be downloaded from the Internet, and then the parameters within the file can be changed as per your need. Alternatively, you can create this file.

In this task, you will perform an unattended installation. To do this, perform the following steps:

_**Step 1**_

Ensure you are connected to **PLABWIN10**.

In the **Type here to search** text box, type the following:

```
windows answer file generator x86
```

Select **Windows answer file generator** from the search results.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-52.jpg?v=18" alt="Figure 2.43 Screenshot of PLABWIN10: Selecting Windows answer file generator Windows 10 from the search results."><figcaption><p>Figure 2.43 Screenshot of PLABWIN10: Selecting Windows answer file generator Windows 10 from the search results.</p></figcaption></figure>

_**Step 2**_

From the search engine results, click the **Windows 10 Answer File Generator for x86 … - windowsafg.com** website link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-53.jpg?v=18" alt="Figure 2.44 Screenshot of PLABWIN10: Selecting Windows answer file generator Windows 10 from the search engine results."><figcaption><p>Figure 2.44 Screenshot of PLABWIN10: Selecting Windows answer file generator Windows 10 from the search engine results.</p></figcaption></figure>

_**Note**: If you are unable to find the link above, stay on the https://windowsafg.com site. Hover your mouse over the **Desktop** menu option. You will see a dropdown list appears. Click on **Windows 10 UEFI** and continue with the lab as intended._

_**Step 3**_

The **Windows Answer File Generator Webpage** is loaded. Scroll down the page and click **Highlight All**.

**Alert:** This web page allows you to create your custom **Autounattend.xml** file. You can either use the default text below the **Highlight All** button, then customize it, or you can customize and download the file.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-54.jpg?v=18" alt="Figure 2.45 Screenshot of PLABWIN10: Clicking the Highlight All button on the Windows Answer File Generator Webpage."><figcaption><p>Figure 2.45 Screenshot of PLABWIN10: Clicking the Highlight All button on the Windows Answer File Generator Webpage.</p></figcaption></figure>

_**Step 4**_

Right-click on the highlighted text and select **Copy** from the context menu.

**Minimize** your browser window.

**Alert:** Please be aware that with this task you are required to toggle off our **Connect device client option**. You will find this option in our **settings page.** For further assistance we recommend you refer to our user guide below:\
**https://docs.practice-labs.com/practice-lab/settings-tab/**\
You will need to reconnect to the device for the change to take effect after toggling the connection client.\
If this is not turned off, you will be disconnected from the device when selecting Copy.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-55.jpg?v=18" alt="Figure 2.46 Screenshot of PLABWIN10: Copying the text on the Windows Answer File Generator Webpage."><figcaption><p>Figure 2.46 Screenshot of PLABWIN10: Copying the text on the Windows Answer File Generator Webpage.</p></figcaption></figure>

_**Step 5**_

Right-click on the desktop and select **Text Document**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-56.jpg?v=18" alt="Figure 2.47 Screenshot of PLABWIN10: Creating a new text document on the desktop."><figcaption><p>Figure 2.47 Screenshot of PLABWIN10: Creating a new text document on the desktop.</p></figcaption></figure>

_**Step 6**_

Click anywhere on the desktop and then double-click **New Text Document**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-57.jpg?v=18" alt="Figure 2.48 Screenshot of PLABWIN10: Opening the text document."><figcaption><p>Figure 2.48 Screenshot of PLABWIN10: Opening the text document.</p></figcaption></figure>

_**Step 7**_

Right-click inside the document and then select **Paste**. This will paste the content into this file.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-58.jpg?v=18" alt="Figure 2.49 Screenshot of PLABWIN10: Pasting the content inside the text document."><figcaption><p>Figure 2.49 Screenshot of PLABWIN10: Pasting the content inside the text document.</p></figcaption></figure>

_**Step 8**_

Click **File** and then select **Save As**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-59.jpg?v=18" alt="Figure 2.50 Screenshot of PLABWIN10: Selecting the Save As option from the File menu."><figcaption><p>Figure 2.50 Screenshot of PLABWIN10: Selecting the Save As option from the File menu.</p></figcaption></figure>

_**Step 9**_

The **Save As** dialog box is displayed. In the **File name** text box, type the following name:

```
Autounattend.xml
```

In the **Save as** type drop-down, select **All Files**. Click **Save**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-60.jpg?v=18" alt="Figure 2.51 Screenshot of PLABWIN10: Saving the file on the desktop as Autounattend.xml."><figcaption><p>Figure 2.51 Screenshot of PLABWIN10: Saving the file on the desktop as Autounattend.xml.</p></figcaption></figure>

_**Step 10**_

Notice that **Autounattend.xml** file is now saved on the desktop.

**Close** the Notepad window. Also, **close** the **Clipboard** dialog box on the upper right corner.

**Alert:** At this point, you are using a sample Autounattend.xml file. You need to ensure that all parameters are properly populated. If it is not done, then the unattended installation will fail and halt where it does not find the correct value. Spend some time going through these values and then proceed further.\
You can refer to the following URL for more help:**https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/automate-windows-setup**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-61.jpg?v=18" alt="Figure 2.52 Screenshot of PLABWIN10: Closing the open windows."><figcaption><p>Figure 2.52 Screenshot of PLABWIN10: Closing the open windows.</p></figcaption></figure>

_**Step 11**_

Select the **New Text Document** file and press **Shift + Delete** to delete the file.

Click **Yes** when prompted for confirmation.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-62.jpg?v=18" alt="Figure 2.53 Screenshot of PLABWIN10: Deleting the New Text Document file."><figcaption><p>Figure 2.53 Screenshot of PLABWIN10: Deleting the New Text Document file.</p></figcaption></figure>

_**Step 12**_

Right-click the **Unattend.xml** file and select **Copy**.

**Close** the **Clipboard** dialog box on the upper right corner if alert should appear.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-63.jpg?v=18" alt="Figure 2.54 Screenshot of PLABWIN10: Copying the Autounattend.xml file."><figcaption><p>Figure 2.54 Screenshot of PLABWIN10: Copying the Autounattend.xml file.</p></figcaption></figure>

_**Step 13**_

Click **File Explorer** from the Windows taskbar.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-64.jpg?v=18" alt="Figure 2.55 Screenshot of PLABWIN10: Opening the File Explorer from the taskbar."><figcaption><p>Figure 2.55 Screenshot of PLABWIN10: Opening the File Explorer from the taskbar.</p></figcaption></figure>

_**Step 14**_

Select **USB (D:)** drive in the left pane. Right-click and select **Paste**.

**Alert:** You can consider the USB (D:) as the **USB drive**. Consider this as a simulated USB drive.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-65.jpg?v=18" alt="Figure 2.56 Screenshot of PLABWIN10: Pasting the file in the selected drive."><figcaption><p>Figure 2.56 Screenshot of PLABWIN10: Pasting the file in the selected drive.</p></figcaption></figure>

_**Step 15**_

Notice that the file is now pasted inside the **USB (D:)** drive.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-66.jpg?v=18" alt="Figure 2.57 Screenshot of PLABWIN10: Showing the pasted file."><figcaption><p>Figure 2.57 Screenshot of PLABWIN10: Showing the pasted file.</p></figcaption></figure>

_**Step 16**_

In the left pane, select **DVD Drive (E**:).

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-67.jpg?v=18" alt="Figure 2.58 Screenshot of PLABWIN10: Selecting the DVD Drive (E:) and displaying its contents."><figcaption><p>Figure 2.58 Screenshot of PLABWIN10: Selecting the DVD Drive (E:) and displaying its contents.</p></figcaption></figure>

_**Step 17**_

Press **Ctrl + A** to select all files. Then, right-click and select **Copy**.

**Close** the **Clipboard** dialog box on the upper right corner if alert should appear.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-68.jpg?v=18" alt="Figure 2.59 Screenshot of PLABWIN10: Selecting and copying all files."><figcaption><p>Figure 2.59 Screenshot of PLABWIN10: Selecting and copying all files.</p></figcaption></figure>

_**Step 18**_

In the left pane, select **USB (D**:). Right-click and then select **Paste**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-69.jpg?v=18" alt="Figure 2.60 Screenshot of PLABWIN10: Pasting the files in the selected drive."><figcaption><p>Figure 2.60 Screenshot of PLABWIN10: Pasting the files in the selected drive.</p></figcaption></figure>

_**Step 19**_

File copying will start. It will take a few minutes to copy the files.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-70.jpg?v=18" alt="Figure 2.61 Screenshot of PLABWIN10: Showing the copy progress."><figcaption><p>Figure 2.61 Screenshot of PLABWIN10: Showing the copy progress.</p></figcaption></figure>

_**Step 20**_

The Windows installation files are now copied to the **USB (D:)** drive.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-71.jpg?v=18" alt="Figure 2.62 Screenshot of PLABWIN10: Showing the pack of files needed for unattended installation"><figcaption><p>Figure 2.62 Screenshot of PLABWIN10: Showing the pack of files needed for unattended installation</p></figcaption></figure>

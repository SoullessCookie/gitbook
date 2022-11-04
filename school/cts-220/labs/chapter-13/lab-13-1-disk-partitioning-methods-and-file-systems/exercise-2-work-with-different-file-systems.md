# Exercise 2 - Work with Different File Systems

### **Exercise 2 - Work with Different File Systems** <a href="#cn-m2-220" id="cn-m2-220"></a>

ExFAT stands for Extended File Allocation Table. ExFAT is ideal for USB flash drives since it is optimized for external storage devices. ExFAT is lightweight and does not have as many features like NTFS. ExFAT doesn’t have the limitations FAT32 does - the maximum file size limitation is much larger in the ExFAT than in FAT32. All modern versions of the Windows operating system and Mac OS extension support ExFAT.

CDFS stands for Compact Disk File Format. CDFS is present in the Linux and Windows operating systems. In Linux, CDFS is used to transfer tracks and bootable images to the compact disk. In windows, CDFS acts as a driver to CD-ROM players. The job of the driver software is to facilitate the use of a CD-ROM drive. Without CDFS being available, it is not possible to use a CD-ROM drive on the Windows operating system.

Ex3 stand for third extended files system and Ex4 stands for the fourth extended file system. Ex3 and Ex4 are Linux file systems. These files systems are not supported on other platforms, like Windows and Mac OS. The maximum file size in Ex3 file system is between 16 GB and 2TB, and in Ex4, it is 16 TB. The maximum volume size in Ex3 is 2 TB to 32 TB. In Ex4, the maximum volume size is 1EB. The maximum number of files that can be stored using the Ex3 system varies. For Ex4 system, this number is 4 billion.

****

**Task 1 - Create FAT32 and NTFS File Systems**

FAT32 is the oldest file system supported by Windows operating system. Most of the USB flash drives are formatted using FAT32 when they are manufactured. FAT32 is ideal for a device that must be used with a variety of other devices, such as computers, televisions sets, games consoles, etc. However, the FAT32 file system has a few limitations. Firstly, the maximum file size in FAT32 system cannot exceed 4GB. Secondly, a maximum drive size in FAT32 system cannot be more than 8TB.

NTFS is the default file system on the recent version of Windows. NTFS has many advantages over FAT32 and ExFAT systems. Some of these features are access rights, backup copies, encryption, and hard links. The partition containing the Windows operating system must be NTFS.

In this exercise, you will learn to create FAT32 and NTFS file systems.

_**Step 1**_

Ensure that the **Disk Management** window is open.

Right-click **New Volume (D:)** and select **Format** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-31.jpg?v=24" alt="Figure 2.1 Screenshot of PLABWIN10: Selecting Format from the context menu."><figcaption><p>Figure 2.1 Screenshot of PLABWIN10: Selecting Format from the context menu.</p></figcaption></figure>

_**Step 2**_

The **Format D:** dialog box is displayed.

Enter the following name in the **Volume label** text box:

```
PLAB
```

From the **File system** drop-down, select **FAT32**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-32.jpg?v=24" alt="Figure 2.2 Screenshot of PLABWIN10: Showing the setting of a volume label and file system in the Format D: dialog box."><figcaption><p>Figure 2.2 Screenshot of PLABWIN10: Showing the setting of a volume label and file system in the Format D: dialog box.</p></figcaption></figure>

_**Step 3**_

Ensure that the **Perform a quick format** checkbox is ticked. Click **OK**.

_**Note:** The Quick Format and Full Format work in the same manner. Both of these format the partition. The only difference is that Quick Format does not check the disk for errors and therefore, formats the partition quickly. On the other hand, the Full Format checks the partition for errors like bad sectors._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-33.jpg?v=24" alt="Figure 2.3 Screenshot of PLABWIN10: Clicking OK on the Format D: dialog box."><figcaption><p>Figure 2.3 Screenshot of PLABWIN10: Clicking OK on the Format D: dialog box.</p></figcaption></figure>

_**Step 4**_

A **Format D:** warning is displayed. Click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-34.jpg?v=24" alt="Figure 2.4 Screenshot of PLABWIN10: Displaying a warning in the Format D: dialog box."><figcaption><p>Figure 2.4 Screenshot of PLABWIN10: Displaying a warning in the Format D: dialog box.</p></figcaption></figure>

_**Step 5**_

You are back on the **Disk Management** window. Notice that the partition is now marked as **PLAB**. Also, notice that the other partitions are marked as **NTFS**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-35.jpg?v=24" alt="Figure 2.5 Screenshot of PLABWIN10: Showing FAT32 and NTFS partitions in Disk Management."><figcaption><p>Figure 2.5 Screenshot of PLABWIN10: Showing FAT32 and NTFS partitions in Disk Management.</p></figcaption></figure>

Minimize the **Disk Management** window.

_**Step 6**_

After creating a FAT32 file system on a partition, you can convert it to the NTFS file system.

In the **Type here to search** text box, type the following command:

```
Cmd
```

Click **Command Prompt**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-36.jpg?v=24" alt="Figure 2.6 Screenshot of PLABWIN10: Command Prompt is shown in the search results."><figcaption><p>Figure 2.6 Screenshot of PLABWIN10: Command Prompt is shown in the search results.</p></figcaption></figure>

_**Step 7**_

The **Administrator: Command Prompt** window is displayed.

Type the following command:

```
convert d: /FS:NTFS
```

Press **Enter**.

**Alert:** You can convert a FAT32 file system to NTFS file system, but you cannot reverse it. You will need to format the partition.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-37.jpg?v=24" alt="Figure 2.7 Screenshot of PLABWIN10: Converting the FAT32 partition to NTFS partition using the convert command."><figcaption><p>Figure 2.7 Screenshot of PLABWIN10: Converting the FAT32 partition to NTFS partition using the convert command.</p></figcaption></figure>

_**Step 8**_

You will be prompted to enter the volume label.

Type the following:

```
PLAB
```

Press **Enter**. Conversion is quick in this case.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-38.jpg?v=24" alt="Figure 2.8 Screenshot of PLABWIN10: Entering the name of the partition to convert and then showing the conversion."><figcaption><p>Figure 2.8 Screenshot of PLABWIN10: Entering the name of the partition to convert and then showing the conversion.</p></figcaption></figure>

**Close** the command prompt window.

_**Step 9**_

Restore the **Disk Management** window. The **D** drive displays **NTFS** instead of **FAT32**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-39.jpg?v=24" alt="Figure 2.9 Screenshot of PLABWIN10: Showing the converted partition as NTFS partition."><figcaption><p>Figure 2.9 Screenshot of PLABWIN10: Showing the converted partition as NTFS partition.</p></figcaption></figure>

#### **Task 2- Configure the Network File System (NFS)** <a href="#cn-m2-293" id="cn-m2-293"></a>

NFS stands for Network File System. NFS makes it possible to share/transfer files from computers running Windows server and Linux operating system by using the NFS protocol. By using NFS, it is possible to access a remote location and use files stored at that location. NFS uses a methodology known as Remote Procedure Call (RPC) to facilitate file transfer. NFS now allows parallel access across multiple servers.

In this task, you will configure NFS.

_**Step 1**_

Connect to **PLABDC01**.

Click the **Start** charm and then select **Server Manager**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-40.jpg?v=24" alt="Figure 2.10 Screenshot of PLABDC01: Selecting Server Manager from the Start menu."><figcaption><p>Figure 2.10 Screenshot of PLABDC01: Selecting Server Manager from the Start menu.</p></figcaption></figure>

_**Step 2**_

The **Server Manager** window is displayed. Click the **Add roles and features** link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-41.jpg?v=24" alt="Figure 2.11 Screenshot of PLABWIN10: Clicking the Add roles and features link."><figcaption><p>Figure 2.11 Screenshot of PLABWIN10: Clicking the Add roles and features link.</p></figcaption></figure>

_**Step 3**_

The **Add Roles and Features Wizard** is displayed.

On the **Before you begin** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-42.jpg?v=24" alt="Figure 2.12 Screenshot of PLABDC01: Showing the Before you begin page in the Add Roles and Features Wizard."><figcaption><p>Figure 2.12 Screenshot of PLABDC01: Showing the Before you begin page in the Add Roles and Features Wizard.</p></figcaption></figure>

_**Step 4**_

On the **Select installation type** page, keep the default selection and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-43.jpg?v=24" alt="Figure 2.13 Screenshot of PLABDC01: Showing the selection of Role-based or feature-based installation option on the Select installation type page."><figcaption><p>Figure 2.13 Screenshot of PLABDC01: Showing the selection of Role-based or feature-based installation option on the Select installation type page.</p></figcaption></figure>

_**Step 5**_

On the **Select destination server** page, keep the default selection and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-44.jpg?v=24" alt="Figure 2.14 Screenshot of PLABDC01: Showing the selection of the server name on the Select destination server page."><figcaption><p>Figure 2.14 Screenshot of PLABDC01: Showing the selection of the server name on the Select destination server page.</p></figcaption></figure>

_**Step 6**_

On the **Select server roles** page, expand **File and Storage Services** and then expand **Files and iSCSI Services**. Tick **Server for NFS**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-45.jpg?v=24" alt="Figure 2.15 Screenshot of PLABDC01: Selecting the Server for NFS option on the Select server roles option."><figcaption><p>Figure 2.15 Screenshot of PLABDC01: Selecting the Server for NFS option on the Select server roles option.</p></figcaption></figure>

_**Step 7**_

The **Add Roles and Features Wizard** dialog box is displayed.

Click **Add Features**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-46.jpg?v=24" alt="Figure 2.16 Screenshot of PLABDC01: Clicking the Add Features button the Add Roles and Features Wizard dialog box."><figcaption><p>Figure 2.16 Screenshot of PLABDC01: Clicking the Add Features button the Add Roles and Features Wizard dialog box.</p></figcaption></figure>

_**Step 8**_

On the **Select server roles** page, notice that **Server for NFS** is now selected. Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-47.jpg?v=24" alt="Figure 2.17 Screenshot of PLABDC01: Showing the selection for Server for NFS option on the Select server roles page."><figcaption><p>Figure 2.17 Screenshot of PLABDC01: Showing the selection for Server for NFS option on the Select server roles page.</p></figcaption></figure>

_**Step 9**_

On the **Select features** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-48.jpg?v=24" alt="Figure 2.18 Screenshot of PLABDC01: Clicking Next on the Select features page."><figcaption><p>Figure 2.18 Screenshot of PLABDC01: Clicking Next on the Select features page.</p></figcaption></figure>

_**Step 10**_

On the **Confirm installation selections** page, click **Install**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-49.jpg?v=24" alt="Figure 2.19 Screenshot of PLABDC01: Clicking Install on the Confirm installation selections page."><figcaption><p>Figure 2.19 Screenshot of PLABDC01: Clicking Install on the Confirm installation selections page.</p></figcaption></figure>

_**Step 11**_

On the **Installation progress** page, the feature installation progress is displayed.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-50.jpg?v=24" alt="Figure 2.20 Screenshot of PLABDC01: Showing the installation on the Installation progress page."><figcaption><p>Figure 2.20 Screenshot of PLABDC01: Showing the installation on the Installation progress page.</p></figcaption></figure>

_**Step 12**_

On the **Installation progress** page, after the installation is completed, click **Close**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-51.jpg?v=24" alt="Figure 2.21 Screenshot of PLABDC01: Clicking Close on the Installation progress page."><figcaption><p>Figure 2.21 Screenshot of PLABDC01: Clicking Close on the Installation progress page.</p></figcaption></figure>

_**Step 13**_

You are back on the **Server Manager** window.

Click the **File and Storage services** link in the left pane.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-52.jpg?v=24" alt="Figure 2.22 Screenshot of PLABDC01: Clicking the File and Storage Service link in the left pane of Server Manager."><figcaption><p>Figure 2.22 Screenshot of PLABDC01: Clicking the File and Storage Service link in the left pane of Server Manager.</p></figcaption></figure>

_**Step 14**_

Ensure that **PLABDC01** is selected in the right pane.

From the sliding menu, click **Shares**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-53.jpg?v=24" alt="Figure 2.23 Screenshot of PLABDC01: Clicking the Shares option in the menu."><figcaption><p>Figure 2.23 Screenshot of PLABDC01: Clicking the Shares option in the menu.</p></figcaption></figure>

_**Step 15**_

Click the **TASKS** drop-down menu and then select **New Share**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-54.jpg?v=24" alt="Figure 2.24 Screenshot of PLABDC01: Selecting the New Share option from the TASKS drop-down."><figcaption><p>Figure 2.24 Screenshot of PLABDC01: Selecting the New Share option from the TASKS drop-down.</p></figcaption></figure>

_**Step 16**_

The **New Share Wizard** is displayed. Select **NFS share - Quick** in the **File share profile** list box.

Then, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-55.jpg?v=24" alt="Figure 2.25 Screenshot of PLABDC01: Selecting the NFS Share - Quick option on the Select the profile for this share page."><figcaption><p>Figure 2.25 Screenshot of PLABDC01: Selecting the NFS Share - Quick option on the Select the profile for this share page.</p></figcaption></figure>

_**Step 17**_

On the **Select the server and path for this share** page, in the **Select by volume** section, select **E**:.

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-56.jpg?v=24" alt="Figure 2.26 Screenshot of PLABDC01: Selecting the E drive on the Select the server and path for this share page."><figcaption><p>Figure 2.26 Screenshot of PLABDC01: Selecting the E drive on the Select the server and path for this share page.</p></figcaption></figure>

_**Step 18**_

On the **Specify share name** page, type the following in the **Share name** text box:

```
Newshare
```

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-57.jpg?v=24" alt="Figure 2.27 Screenshot of PLABDC01: Specifying the name in the Share name text box on the Specify share name page."><figcaption><p>Figure 2.27 Screenshot of PLABDC01: Specifying the name in the Share name text box on the Specify share name page.</p></figcaption></figure>

_**Step 19**_

On the **Specify authentication methods** page, tick **No server authentication (AUTH\_SYS**), then tick **Enable unmapped user access** and **Allow anonymous access**.

_We are allowing the minimum authentication required to simplify the share point access for other host machines._

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-58.jpg?v=24" alt="Figure 2.28 Screenshot of PLABDC01: Selecting the No server authentication (AUTH_SYS), Enable unmapped user access and Allow anonymous access options."><figcaption><p>Figure 2.28 Screenshot of PLABDC01: Selecting the No server authentication (AUTH_SYS), Enable unmapped user access and Allow anonymous access options.</p></figcaption></figure>

_**Step 20**_

On the **Server Authentication** warning message, select **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-59.jpg?v=24" alt="Figure 2.29 Screenshot of PLABDC01: Clicking Yes on the Server Authentication warning message."><figcaption><p>Figure 2.29 Screenshot of PLABDC01: Clicking Yes on the Server Authentication warning message.</p></figcaption></figure>

_**Step 21**_

On the **Specify the share permissions** page, click **Add**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-60.jpg?v=24" alt="Figure 2.30 Screenshot of PLABDC01: Clicking Add on the Specify the share permissions page."><figcaption><p>Figure 2.30 Screenshot of PLABDC01: Clicking Add on the Specify the share permissions page.</p></figcaption></figure>

_**Step 22**_

On the **Add Permissions** page, in the **Hosts** text box, type **192.168.0.2**.

Click the **Share permissions** dropdown, select **Read / Write**.

Click **Add**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-61.jpg?v=24" alt="Figure 2.31 Screenshot of PLABDC01: Adding Host 192.168.0.2 to the permitted machines to access the NFS share."><figcaption><p>Figure 2.31 Screenshot of PLABDC01: Adding Host 192.168.0.2 to the permitted machines to access the NFS share.</p></figcaption></figure>

_**Step 23**_

Back on the **Specify the share permissions** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-62.jpg?v=24" alt="Figure 2.32 Screenshot of PLABDC01: Clicking next on the Specify the share permissions page."><figcaption><p>Figure 2.32 Screenshot of PLABDC01: Clicking next on the Specify the share permissions page.</p></figcaption></figure>

_**Step 24**_

On the **Specify permissions to control access page**, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-63.jpg?v=24" alt="Figure 2.33 Screenshot of PLABDC01: Clicking next on the Specify permissions to control access page."><figcaption><p>Figure 2.33 Screenshot of PLABDC01: Clicking next on the Specify permissions to control access page.</p></figcaption></figure>

_**Step 25**_

On the **Specify permissions to control access** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-64.jpg?v=24" alt="Figure 2.34 Screenshot of PLABDC01: Clicking next on the Specify permissions to control access page."><figcaption><p>Figure 2.34 Screenshot of PLABDC01: Clicking next on the Specify permissions to control access page.</p></figcaption></figure>

_**Step 26**_

On the **Confirm selections** page, click **Create** to create an NFS share.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-65.jpg?v=24" alt="Figure 2.35 Screenshot of PLABDC01: Clicking Create on the Confirm selections page."><figcaption><p>Figure 2.35 Screenshot of PLABDC01: Clicking Create on the Confirm selections page.</p></figcaption></figure>

_**Step 27**_

On the **View results** page, click **Close**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-66.jpg?v=24" alt="Figure 2.36 Screenshot of PLABDC01: Clicking Close on the View results page."><figcaption><p>Figure 2.36 Screenshot of PLABDC01: Clicking Close on the View results page.</p></figcaption></figure>

_**Step 28**_

Now you have created an NFS share on the E: drive of PLABDC01.

Let’s now connect to the NFS share from **PLABWIN10**.

Connect to the **PLABWIN10** device.

Open **File Explorer** from the Windows taskbar.

From the left pane, right-click **This PC** and select **Map network drive…** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-67.jpg?v=24" alt="Figure 2.37 Screenshot of PLABWIN10: Mapping a new network drive to the PLABWIN10 device."><figcaption><p>Figure 2.37 Screenshot of PLABWIN10: Mapping a new network drive to the PLABWIN10 device.</p></figcaption></figure>

_**Step 29**_

The **Map Network Drive** dialog box is displayed.

In the **Folder** drop-down, type the following path:

```
\\plabdc01\E\Shares\Newshare
```

Click **Finish**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-68.jpg?v=24" alt="Figure 2.38 Screenshot of PLABWIN10: Entering the path in the Folder drop-down on the Map Network Drive dialog box."><figcaption><p>Figure 2.38 Screenshot of PLABWIN10: Entering the path in the Folder drop-down on the Map Network Drive dialog box.</p></figcaption></figure>

_**Step 30**_

A new **File Explorer** window is displayed. You have successfully connected with the NFS share.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-69.jpg?v=24" alt="Figure 2.39 Screenshot of PLABWIN10: Showing the share that is accessible."><figcaption><p>Figure 2.39 Screenshot of PLABWIN10: Showing the share that is accessible.</p></figcaption></figure>

_**Step 31**_

**Close** all open windows.

#### **Task 3 - View the Swap Partition on CentOS** <a href="#cn-m2-439" id="cn-m2-439"></a>

A swap partition is a part of the hard disk space. This space is used as an extension of the RAM in a computer system. The swap partition is a way to overcome RAM limitations of your system.

When applications demand memory, and there is no physical memory available, then the swap partition is used. The swap partition works like additional memory in the system. However, it is important to note that a swap partition is NOT the replacement for physical memory.

The most recently used files are in the RAM, and the least recently used files are kept in the swap partition. When a new file is to be swapped into the RAM, the least recently used file is swapped out of it and moved to the swap partition.

A swap partition is created on the hard drive, and therefore, it can increase the wear and tear of the hard drive.

In this task, you will view the swap partition in CentOS.

_**Step 1**_

Connect to **PLABCENTOS**.

On the desktop, right-click and select **Open Terminal**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-70.jpg?v=24" alt="Figure 2.40 Screenshot of PLABCENTOS: Selecting the Open Terminal option from the context menu."><figcaption><p>Figure 2.40 Screenshot of PLABCENTOS: Selecting the Open Terminal option from the context menu.</p></figcaption></figure>

_**Step 2**_

The terminal window is displayed. Type the following command:

```
su -
```

Press **Enter**.

At the **Password** prompt, type the following password:

Passw0rd

Press **Enter**.

_**Step 3**_

To view the swap partition, type the following command:

```
swapon -s
```

Press **Enter**. Notice that CentOS has a **209174 KB** of the swap partition. This number may vary in the lab enviroment.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-72.jpg?v=24" alt="Figure 2.42 Screenshot of PLABCENTOS: viewing the swap partition with the swapon -s command."><figcaption><p>Figure 2.42 Screenshot of PLABCENTOS: viewing the swap partition with the swapon -s command.</p></figcaption></figure>

#### **Task 4 - View the Swap File in Windows 10** <a href="#cn-m2-465" id="cn-m2-465"></a>

Windows does not contain a swap partition, but it contains a swap file, which is known as pagefile.sys. It serves the same purpose as the swap partition. You can store the pagefile.sys in its default location, create a new partition and store the pagefile.sys there, or configure the pagefile.sys to be stored on all partitions.

In this task, you will view the swap partition in Windows 10.

_**Step 1**_

Connect back to **PLABWIN10**. In the Type here to search text box, type the following command:

```
Control Panel
```

Select **Control Panel** from the search results.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-73.jpg?v=24" alt="Figure 2.43 Screenshot of PLABWIN10: Selecting Control Panel from the search results."><figcaption><p>Figure 2.43 Screenshot of PLABWIN10: Selecting Control Panel from the search results.</p></figcaption></figure>

_**Step 2**_

The **Control Panel** window is displayed. Select **System and Security.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-74.jpg?v=24" alt="Figure 2.44 Screenshot of PLABWIN10: Selecting System and Security from the Control Panel window."><figcaption><p>Figure 2.44 Screenshot of PLABWIN10: Selecting System and Security from the Control Panel window.</p></figcaption></figure>

_**Step 3**_

Click **System** from the **System and Security** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-75.jpg?v=24" alt="Figure 2.45 Screenshot of PLABWIN10: Selecting System from the System and Security window."><figcaption><p>Figure 2.45 Screenshot of PLABWIN10: Selecting System from the System and Security window.</p></figcaption></figure>

_**Step 4**_

The **System** window is displayed. In the left pane, click the **Advanced system settings** link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-76.jpg?v=24" alt="Figure 2.46 Screenshot of PLABWIN10: Clicking the Advanced system settings link in the left pane."><figcaption><p>Figure 2.46 Screenshot of PLABWIN10: Clicking the Advanced system settings link in the left pane.</p></figcaption></figure>

_**Step 5**_

The **System Properties** dialog box is displayed. On the **Advanced** tab, click **Settings** in the **Performance** section.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-77.jpg?v=24" alt="Figure 2.47 Screenshot of PLABWIN10: Clicking Settings on the Advanced tab of the System Properties dialog box."><figcaption><p>Figure 2.47 Screenshot of PLABWIN10: Clicking Settings on the Advanced tab of the System Properties dialog box.</p></figcaption></figure>

_**Step 6**_

The **Performance Options** dialog box is displayed. Click the **Advanced** tab, and then click **Change** in the **Virtual memory** section.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-78.jpg?v=24" alt="Figure 2.48 Screenshot of PLABWIN10: Clicking Change on the Advanced tab of the Performance Options dialog box."><figcaption><p>Figure 2.48 Screenshot of PLABWIN10: Clicking Change on the Advanced tab of the Performance Options dialog box.</p></figcaption></figure>

_**Step 7**_

The **Virtual Memory** dialog box is displayed.

Notice that **Automatically manage paging file size for all drives** is selected by default. When this option is selected, there is no manual intervention required to set the paging file size. Windows, depending on the RAM installed, configures the size of the **pagefile.sys** file.

If you deselect this option, then you should select the **Custom size** and set the page file size on a single partition or multiple partitions/hard drives.

Also notice that the **Total paging file size for all drives** is displayed in the **Virtual memory** section.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-79.jpg?v=24" alt="Figure 2.49 Screenshot of PLABWIN10: Showing the Virtual Memory dialog box with the page file configuration."><figcaption><p>Figure 2.49 Screenshot of PLABWIN10: Showing the Virtual Memory dialog box with the page file configuration.</p></figcaption></figure>

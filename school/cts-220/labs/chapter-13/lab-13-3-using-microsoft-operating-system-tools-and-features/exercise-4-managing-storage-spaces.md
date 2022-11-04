# Exercise 4 - Managing Storage Spaces

### **Exercise 4 - Managing Storage Spaces** <a href="#cn-m5-622" id="cn-m5-622"></a>

**Disk Management** is a GUI-based Windows tool introduced in Windows XP and available in all later versions. **Disk Management** helps create, format, and manage disks, both internal and external. You can use the **Disk Management** tool to create and attach hard disks, view and format various disks configured on the system, list the storage space configured on the hard drives and view the free space available.

Windows also provides the **Storage Spaces** feature that helps create a pool of disk drives. This pool can then be used to provide data redundancy as well as memory flexibility on the computer.



#### **Task 1 - Initialize a Disk** <a href="#cn-m5-638" id="cn-m5-638"></a>

After adding a disk to a computer, you need to initialize the disk to make it discoverable by the OS. An initialized disk can then be partitioned or formatted to make it ready for storing data. The **Disk Management** tool enables you to bring disks online to make them available for initialization.

In this task, you will use the **Disk Management** tool to bring a disk online.

_**Step 1**_

Ensure that **PLABWIN10** is running and the desktop is displayed.

In the **Type here to search** textbox in the taskbar and type the following:

```
Disk Management
```

Under **Best Match** section, select **Create and format hard disk partitions**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-82.jpg?v=29" alt="Figure 4.1 Screenshot of PLABWIN10: Selecting Create and format hard disk partitions from the search results."><figcaption><p>Figure 4.1 Screenshot of PLABWIN10: Selecting Create and format hard disk partitions from the search results.</p></figcaption></figure>

_**Step 2**_

The **Disk Management** window is displayed.

Notice that the disks configured on the computer, along with the relevant details are listed. **Disk 1** is currently marked as **Online**.

In the bottom pane, right-click in the **Disk 1** section on the left and select **Offline**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-83.jpg?v=29" alt="Figure 4.2 Screenshot of PLABWIN10: Making Disk 1 offline."><figcaption><p>Figure 4.2 Screenshot of PLABWIN10: Making Disk 1 offline.</p></figcaption></figure>

_**Step 3**_

**Disk 1** is now marked as **Offline**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-84.jpg?v=29" alt="Figure 4.3 Screenshot of PLABWIN10: Showing Disk 1 as offline."><figcaption><p>Figure 4.3 Screenshot of PLABWIN10: Showing Disk 1 as offline.</p></figcaption></figure>

_**Step 4**_

To bring the disk online, right-click in the **Disk 1** section on the left and select **Online**.

_**Note**: You can use these steps to convert any offline disk to online, irrespective of its initial status._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-85.jpg?v=29" alt="Figure 4.4 Screenshot of PLABWIN10: Selecting Online from the context menu of Disk 1."><figcaption><p>Figure 4.4 Screenshot of PLABWIN10: Selecting Online from the context menu of Disk 1.</p></figcaption></figure>

_**Step 5**_

Notice that **Disk 1** is now marked as **Online**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-86.jpg?v=29" alt="Figure 4.5 Screenshot of PLABWIN10: Showing Disk 1 as Online."><figcaption><p>Figure 4.5 Screenshot of PLABWIN10: Showing Disk 1 as Online.</p></figcaption></figure>

_**Step 6**_

To partition and format the drives, the drives must be dynamic.

To make **Disk 1** dynamic, right-click in the **Disk 1** section on the left and select **Convert to Dynamic Disk.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-87.jpg?v=29" alt="Figure 4.6 Screenshot of PLABWIN10: Selecting Convert to Dynamic Disk from the context menu of Disk 1."><figcaption><p>Figure 4.6 Screenshot of PLABWIN10: Selecting Convert to Dynamic Disk from the context menu of Disk 1.</p></figcaption></figure>

_**Step 7**_

The **Convert to Dynamic Disk** dialog box is displayed.

Ensure that the **Disk 1** checkbox is selected by default.

Click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-88.jpg?v=29" alt="Figure 4.7 Screenshot of PLABWIN10: Showing the Convert to Dynamic Disk dialog box with Disk 1 selected."><figcaption><p>Figure 4.7 Screenshot of PLABWIN10: Showing the Convert to Dynamic Disk dialog box with Disk 1 selected.</p></figcaption></figure>

_**Step 8**_

The **Disks to Convert** dialog box is displayed. It displays **Disk 1** for conversion.

Click **Convert**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-89.jpg?v=29" alt="Figure 4.8 Screenshot of PLABWIN10: Clicking the Convert button on the Disk to Convert dialog box."><figcaption><p>Figure 4.8 Screenshot of PLABWIN10: Clicking the Convert button on the Disk to Convert dialog box.</p></figcaption></figure>

_**Step 9**_

The **Disk Management** dialog box is displayed listing the effects of converting the disks.

Click **Yes** proceed with the conversion.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-90.jpg?v=29" alt="Figure 4.9 Screenshot of PLABWIN10: Showing  confirmation to proceed with the conversion and showing the Yes button highlighted."><figcaption><p>Figure 4.9 Screenshot of PLABWIN10: Showing confirmation to proceed with the conversion and showing the Yes button highlighted.</p></figcaption></figure>

_**Step 10**_

Back on the **Disk Management** console, notice the **Healthy (Primary partition)** status of **Disk 1** now changes to **Healthy**. This indicates that the disk is now dynamic and available for portioning and formatting.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-91.jpg?v=29" alt="Figure 4.10 Screenshot of PLABWIN10: Showing the updated status of the newly converted disk."><figcaption><p>Figure 4.10 Screenshot of PLABWIN10: Showing the updated status of the newly converted disk.</p></figcaption></figure>

#### **Task 2 - Partition a Dynamic Disk** <a href="#cn-m5-692" id="cn-m5-692"></a>

**Disk Management** tool enables you to partition dynamic disks and create volumes in various formats. It provides GUI options to create disks in simple, spanned, striped, mirrored, and RAID-level formats.

In this task, you will use the **Disk Management** tool to format a disk to create a simple volume.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **Disk Management** console is displayed.

Right-click **Disk 1** and select **Delete Volume** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-92.jpg?v=29" alt="Figure 4.11 Screenshot of PLABWIN10: Selecting Delete Volume from the context menu of Disk 1."><figcaption><p>Figure 4.11 Screenshot of PLABWIN10: Selecting Delete Volume from the context menu of Disk 1.</p></figcaption></figure>

_**Step 2**_

The **Delete simple volume** dialog box is displayed. Click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-93.jpg?v=29" alt="Figure 4.12 Screenshot of PLABWIN10: Confirming the deletion of volume."><figcaption><p>Figure 4.12 Screenshot of PLABWIN10: Confirming the deletion of volume.</p></figcaption></figure>

_**Step 3**_

Notice that **Disk 1** is now marked as **Unallocated**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-94.jpg?v=29" alt="Figure 4.13 Screenshot of PLABWIN10: Showing Disk 1 as Unallocated."><figcaption><p>Figure 4.13 Screenshot of PLABWIN10: Showing Disk 1 as Unallocated.</p></figcaption></figure>

_**Step 4**_

Right-click **Disk 1** and select **New Simple Volume**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-95.jpg?v=29" alt="Figure 4.14 Screenshot of PLABWIN10: Selecting New Simple Volume from the context menu of Disk 1."><figcaption><p>Figure 4.14 Screenshot of PLABWIN10: Selecting New Simple Volume from the context menu of Disk 1.</p></figcaption></figure>

_**Step 5**_

The **New Simple Volume Wizard** is displayed.

On the **Welcome to the New Simple Volume Wizard** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-96.jpg?v=29" alt="Figure 4.15 Screenshot of PLABWIN10: Showing the Welcome page on the New Simple Volume Wizard."><figcaption><p>Figure 4.15 Screenshot of PLABWIN10: Showing the Welcome page on the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 6**_

On the **Specify Volume Size** page, accept the default settings and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-97.jpg?v=29" alt="Figure 4.16 Screenshot of PLABWIN10: Specifying the Volume Size page on the New Simple Volume Wizard."><figcaption><p>Figure 4.16 Screenshot of PLABWIN10: Specifying the Volume Size page on the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 7**_

On the **Assign Drive Letter or Path** page, select the **Assign the following drive letter** checkbox.

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-98.jpg?v=29" alt="Figure 4.17 Screenshot of PLABWIN10: Selecting Assign the following drive letter on the New Simple Volume Wizard."><figcaption><p>Figure 4.17 Screenshot of PLABWIN10: Selecting Assign the following drive letter on the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 8**_

On the **Format Partition** page, keep the **Format this volume with the following settings** option selected. In the **Volume label** textbox, type the following name:

```
Data
```

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-99.jpg?v=29" alt="Figure 4.18 Screenshot of PLABWIN10: Showing the Format Partition page on the New Simple Volume Wizard with Data as the Volume label."><figcaption><p>Figure 4.18 Screenshot of PLABWIN10: Showing the Format Partition page on the New Simple Volume Wizard with Data as the Volume label.</p></figcaption></figure>

_**Step 9**_

On the **Completing the New Simple Volume Wizard** page, review the details and click **Finish**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-100.jpg?v=29" alt="Figure 4.19 Screenshot of PLABWIN10: Showing the Completion page on the New Simple Volume Wizard listing specifications to create the volume."><figcaption><p>Figure 4.19 Screenshot of PLABWIN10: Showing the Completion page on the New Simple Volume Wizard listing specifications to create the volume.</p></figcaption></figure>

_**Step 10**_

Notice that a new simple volume has been created on **Disk 1** and it has been labeled as **Data**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-101.jpg?v=29" alt="Figure 4.20 Screenshot of PLABWIN10: Showing the newly created volume with Data as the label."><figcaption><p>Figure 4.20 Screenshot of PLABWIN10: Showing the newly created volume with Data as the label.</p></figcaption></figure>

#### **Task 3 - Explore Disk Management Operations** <a href="#cn-m5-740" id="cn-m5-740"></a>

The **Disk Management** tool supports management operations such as listing the properties of a selected disk, extending/shrinking a volume, changing the letter or path assigned to a drive. In this task, you will explore these disk management operations available on the tool.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **Disk Management** console is displayed.

You will now view the properties of the **Data (D:)** drive. To do this, right-click **Data (D:)** and select **Properties**.

On the context-menu displayed, select **Properties**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-102.jpg?v=29" alt="Figure 4.21 Screenshot of PLABWIN10: Selecting Properties from the context menu of the Disk 1."><figcaption><p>Figure 4.21 Screenshot of PLABWIN10: Selecting Properties from the context menu of the Disk 1.</p></figcaption></figure>

_**Step 2**_

The **Data (D:) Properties** dialog box is displayed.

There are various tasks that can be performed in this dialog box. For this task, you will not make any changes. Click **Cancel** to close the dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-103.jpg?v=29" alt="Figure 4.22 Screenshot of PLABWIN10: Showing the Properties dialog box."><figcaption><p>Figure 4.22 Screenshot of PLABWIN10: Showing the Properties dialog box.</p></figcaption></figure>

_**Step 3**_

You will now extend the volume of the **Data (D:)** drive.

Again, right-click the drive and select **Extend Volume.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-104.jpg?v=29" alt="Figure 4.23 Screenshot of PLABWIN10: Selecting the Extend Volume from the context menu of Disk 1."><figcaption><p>Figure 4.23 Screenshot of PLABWIN10: Selecting the Extend Volume from the context menu of Disk 1.</p></figcaption></figure>

_**Step 4**_

The **Extend Volume Wizard** is displayed.

On the **Welcome to the Extend Volume** Wizard page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-105.jpg?v=29" alt="Figure 4.24 Screenshot of PLABWIN10: Showing the Welcome page on the Extend Volume Wizard."><figcaption><p>Figure 4.24 Screenshot of PLABWIN10: Showing the Welcome page on the Extend Volume Wizard.</p></figcaption></figure>

_**Step 5**_

On the **Select Disks** page, select **Disk 2** from the **Available** panel list and click **Add**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-106.jpg?v=29" alt="Figure 4.25 Screenshot of PLABWIN10: Showing the Select Disks page on the Extend Volume Wizard."><figcaption><p>Figure 4.25 Screenshot of PLABWIN10: Showing the Select Disks page on the Extend Volume Wizard.</p></figcaption></figure>

_**Step 5**_

Notice that the disk is now added to the **Selected** list.

In the **Select the amount of space in MB** textbox, type the following size:

```
10 
```

This specifies that the disk **D:** is to be extended by 10 MB. Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-107.jpg?v=29" alt="Figure 4.26 Screenshot of PLABWIN10: Showing the Select Disks page on the Extend Volume Wizard."><figcaption><p>Figure 4.26 Screenshot of PLABWIN10: Showing the Select Disks page on the Extend Volume Wizard.</p></figcaption></figure>

_**Step 6**_

On the **Completing the Extend Volume Wizard** page, click **Finish**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-108.jpg?v=29" alt="Figure 4.27 Screenshot of PLABWIN10: Showing the Completion page on the Extend Volume Wizard."><figcaption><p>Figure 4.27 Screenshot of PLABWIN10: Showing the Completion page on the Extend Volume Wizard.</p></figcaption></figure>

_**Step 7**_

The **Disk Management** dialog box appears warning that the specified operation will convert the disk into a dynamic disk, which might complicate the booting process of the machine.

Click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-109.jpg?v=29" alt="Figure 4.28 Screenshot of PLABWIN10: Showing the Disk Management dialog box for confirmation to proceed with extending the volume."><figcaption><p>Figure 4.28 Screenshot of PLABWIN10: Showing the Disk Management dialog box for confirmation to proceed with extending the volume.</p></figcaption></figure>

_**Step 8**_

Note that the **Data (D:)** volume is now extended.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-110.jpg?v=29" alt="Figure 4.29 Screenshot of PLABWIN10: Showing the Disk Management window with the extended disk."><figcaption><p>Figure 4.29 Screenshot of PLABWIN10: Showing the Disk Management window with the extended disk.</p></figcaption></figure>

_**Step 9**_

Just as you extended the volume, you can shrink a volume as well.

Right-click the **Data (D:)** drive and select **Shrink Volume**.

If you encounter an error, search Windows for the Command Prompt and enter the following command “sc config defragsvc start=auto” which should return a success and then reattempt the step.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-111.jpg?v=29" alt="Figure 4.30 Screenshot of PLABWIN10: Selecting Shrink Volume from the context menu of Disk 1."><figcaption><p>Figure 4.30 Screenshot of PLABWIN10: Selecting Shrink Volume from the context menu of Disk 1.</p></figcaption></figure>

_**Step 10**_

The **Shrink** dialog box is displayed.

Keep the default values and click **Shrink**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-112.jpg?v=29" alt="Figure 4.31 Screenshot of PLABWIN10: Showing the Shrink D: dialog box and showing the Shrink button highlighted."><figcaption><p>Figure 4.31 Screenshot of PLABWIN10: Showing the Shrink D: dialog box and showing the Shrink button highlighted.</p></figcaption></figure>

_**Step 11**_

Notice that the **Data (D:)** is now shrunk.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-113.jpg?v=29" alt="Figure 4.32 Screenshot of PLABWIN10: Showing the shrunk Disk 1."><figcaption><p>Figure 4.32 Screenshot of PLABWIN10: Showing the shrunk Disk 1.</p></figcaption></figure>

#### **Task 4 - Re-initialize a Disk** <a href="#cn-m5-802" id="cn-m5-802"></a>

You might have to change the letter assigned to a drive. This might be required in case of an automatically assigned drive letter, or while mapping a network drive to another computer. **Disk Management** enables you to re-initialize a drive by changing the letter assigned to it or by changing its path.

In this task, you will use the **Disk Management** tool to re-initialize a drive.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **Disk Management** console is displayed.

In the top pane, right-click **Data** (**D:)** and select the **Change Drive Letter and Paths…** option.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-114.jpg?v=29" alt="Figure 4.33 Screenshot of PLABWIN10: Selecting Change Drive Letter or Paths from the context menu of Disk 1."><figcaption><p>Figure 4.33 Screenshot of PLABWIN10: Selecting Change Drive Letter or Paths from the context menu of Disk 1.</p></figcaption></figure>

_**Step 2**_

The **Change Drive Letter and Paths** dialog box is displayed. Click **Change.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-115.jpg?v=29" alt="Figure 4.34 Screenshot of PLABWIN10: Showing the Change Drive Letter and Paths for D: (Data) dialog box is displayed showing the required disk selected, and the Change button highlighted."><figcaption><p>Figure 4.34 Screenshot of PLABWIN10: Showing the Change Drive Letter and Paths for D: (Data) dialog box is displayed showing the required disk selected, and the Change button highlighted.</p></figcaption></figure>

_**Step 3**_

From the **Assign the following drive letter** drop-down list, select **K**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-116.jpg?v=29" alt="Figure 4.35 Screenshot of PLABWIN10: Showing the Change Drive Letter or Path dialog box is displayed showing the required drive letter selected."><figcaption><p>Figure 4.35 Screenshot of PLABWIN10: Showing the Change Drive Letter or Path dialog box is displayed showing the required drive letter selected.</p></figcaption></figure>

_**Step 4**_

Click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-117.jpg?v=29" alt="Figure 4.36 Screenshot of PLABWIN10: Change Drive Letter or Path dialog box is displayed showing the OK button highlighted."><figcaption><p>Figure 4.36 Screenshot of PLABWIN10: Change Drive Letter or Path dialog box is displayed showing the OK button highlighted.</p></figcaption></figure>

_**Step 5**_

On the **Disk Management** dialog box, click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-118.jpg?v=29" alt="Figure 4.37 Screenshot of PLABWIN10: Clicking Yes on the Disk Management dialog box."><figcaption><p>Figure 4.37 Screenshot of PLABWIN10: Clicking Yes on the Disk Management dialog box.</p></figcaption></figure>

_**Step 6**_

Notice that the instead of **Data (D**:), it is now marked as **Data (K**:).

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-119.jpg?v=29" alt="Figure 4.38 Screenshot of PLABWIN10: Showing the updated drive letter for Disk 1."><figcaption><p>Figure 4.38 Screenshot of PLABWIN10: Showing the updated drive letter for Disk 1.</p></figcaption></figure>

#### **Task 5 - Manage Storage Spaces** <a href="#cn-m5-830" id="cn-m5-830"></a>

The **Storage Spaces** feature enables you to create a storage pool by grouping two or more drives into a storage pool. On this pool, you can configure virtual drives known as the “storage spaces”. By default, the storage spaces store two copies of every file saved, thereby providing redundancy and ensuring data availability. Moreover, you can use the storage space pool to provide for any additional storage space requirements on the computer. You can even add more drives to extend the pool capacity.

In this task, you will create a **Storage Space** using **Disk 1** and **Disk 2** on the computer.

_**Step 1**_

In the Disk Management window, delete the existing partitions for **Disk 1** and **Disk 2**. Then, create simple volumes on both the disks.

Minimize the **Disk Management** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-120.jpg?v=29" alt="Figure 4.39 Screenshot of PLABWIN10: Showing the updated drives in the Disk Management window."><figcaption><p>Figure 4.39 Screenshot of PLABWIN10: Showing the updated drives in the Disk Management window.</p></figcaption></figure>

_**Step 2**_

Ensure that **PLABWIN10** is running. Access the desktop.

In the **Type here to search** textbox in the taskbar and type the following:

```
Storage Spaces  
```

Under **Best Match** section, select **Manage Storage Spaces**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-121.jpg?v=29" alt="Figure 4.40 Screenshot of PLABWIN10: Selecting Manage Storage Spaces from the search result."><figcaption><p>Figure 4.40 Screenshot of PLABWIN10: Selecting Manage Storage Spaces from the search result.</p></figcaption></figure>

_**Step 3**_

The **Storage Spaces** window is displayed.

On the **Manage Storage Spaces** page, select the **Create a new pool and storage space** link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-122.jpg?v=29" alt="Figure 4.41 Screenshot of PLABWIN10: Clicking the Create a new pool and storage space link on the Manage Storage Spaces page."><figcaption><p>Figure 4.41 Screenshot of PLABWIN10: Clicking the Create a new pool and storage space link on the Manage Storage Spaces page.</p></figcaption></figure>

_**Step 4**_

On the **Select drives to create a storage pool** page, select both of the drives and click **Create pool**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-123.jpg?v=29" alt="Figure 4.42 Screenshot of PLABWIN10: Showing the Select drives to create storage pool page on the Create a storage pool window showing the required selections performed and the Create pool button highlighted."><figcaption><p>Figure 4.42 Screenshot of PLABWIN10: Showing the Select drives to create storage pool page on the Create a storage pool window showing the required selections performed and the Create pool button highlighted.</p></figcaption></figure>

_**Note:** If no disks are available to select, please make sure you have recreated the volumes in Task 5, Step 1_

_**Step 5**_

The **Create a Storage Pool** dialog box is displayed.

Click **Close**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-124.jpg?v=29" alt="Figure 4.43 Screenshot of PLABWIN10: Showing an error in the Create a Storage Pool dialog box."><figcaption><p>Figure 4.43 Screenshot of PLABWIN10: Showing an error in the Create a Storage Pool dialog box.</p></figcaption></figure>

_**Step 6**_

The **Create a storage space** window is displayed.

On the **Enter a name, resiliency type, and size for the storage space** page, input the following settings:

Set the **Resiliency type** drop-down list box to **Simple (no resiliency**).

In the **Size (maximum)** text box, change the size to **4.00 GB**.

Click **Create storage space**.

_**Note:** If the Create storage space is greyed out please press cancel and continue to the next step._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-125.jpg?v=29" alt="Figure 4.44 Screenshot of PLABWIN10: Making configuration changes for creating storage space."><figcaption><p>Figure 4.44 Screenshot of PLABWIN10: Making configuration changes for creating storage space.</p></figcaption></figure>

_**Step 7**_

Back on the **Manage Storage Spaces** page on the **Storage Spaces** window, notice that the newly created storage pool is now listed along with the capacity, usage, and disk details.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-126.jpg?v=29" alt="Figure 4.45 Screenshot of PLABWIN10: Showing the newly created storage pool."><figcaption><p>Figure 4.45 Screenshot of PLABWIN10: Showing the newly created storage pool.</p></figcaption></figure>

# Exercise 1 - Perform Disk Partitioning



### **Exercise 1 - Perform Disk Partitioning** <a href="#cn-m2-44" id="cn-m2-44"></a>

Disk partitioning is performed to create logically separate compartments inside the hard drive.

There are three types of disk partitions: Primary, logical and extended. A hard drive can have a maximum of four primary partitions or three primary and one extended partition. Logical partitions are created on the extended partition. The primary partition with the ACTIVE status is used for booting the system with an operating system. You cannot boot a system from a logical partition as it cannot be made ACTIVE.

Disk partitions are useful from a data security point of view. Formatting and erasing data from one partition does not affect the data stored in another partition. If the hard drive with multiple partitions fails, the data on all partitions is impacted.



**Task 1 - Create a Dynamic Partition**

A basic disk works with partitions. Each partition is independent and cannot share or span data over other partitions. A dynamic disk can use dynamic volumes that can span across multiple hard drives in a single system.

This is possible because the dynamic disk partition does not create a partition table like the regular partition method. Dynamic partitioning uses a method called logical disk manager (LDM). LDM keeps track of the sectors of the dynamic partition. A basic disk can be converted to dynamic disk and vice versa.

In this task you will create a dynamic partition.

_**Step 1**_

Ensure that the required devices are powered on and connect to **PLABWIN10**.

In the **Type here to search** text box, type the following:

```
Disk management
```

Select the **Create and format hard disk partitions** from the search results.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-2.jpg?v=24" alt="Figure 1.1 Screenshot of PLABWIN10: Selecting Create and format hard disk partitions from the search results."><figcaption><p>Figure 1.1 Screenshot of PLABWIN10: Selecting Create and format hard disk partitions from the search results.</p></figcaption></figure>

_**Step 2**_

The **Disk Management** window is displayed.

On the left hand side of the lower pane, right-click **Disk 1** and select **Convert to Dynamic Disk** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-3.jpg?v=24" alt="Figure 1.2 Screenshot of PLABWIN10: Right-clicking Disk 1 and selecting Convert to Dynamic Disk from the context menu."><figcaption><p>Figure 1.2 Screenshot of PLABWIN10: Right-clicking Disk 1 and selecting Convert to Dynamic Disk from the context menu.</p></figcaption></figure>

_**Step 3**_

The **Convert to Dynamic Disk** dialog box is displayed.

Ensure that **Disk 1** is selected. Click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-4.jpg?v=24" alt="Figure 1.3 Screenshot of PLABWIN10: Selecting e disk drive to convert to a dynamic disk in the Disk Management."><figcaption><p>Figure 1.3 Screenshot of PLABWIN10: Selecting e disk drive to convert to a dynamic disk in the Disk Management.</p></figcaption></figure>

_**Step 4**_

The **Disk to Convert** dialog box is displayed.

Click **Convert**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-5.jpg?v=24" alt="Figure 1.4 Screenshot of PLABWIN10: Clicking the Convert button in the Disks to Convert dialog box."><figcaption><p>Figure 1.4 Screenshot of PLABWIN10: Clicking the Convert button in the Disks to Convert dialog box.</p></figcaption></figure>

_**Step 5**_

Notice that the **Disk 1** status is set to **Basic**.

The **Disk Management** dialog box is displayed.

Click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-6.jpg?v=24" alt="Figure 1.5 Screenshot of PLABWIN10: Showing the warning message in the Disk Management dialog box."><figcaption><p>Figure 1.5 Screenshot of PLABWIN10: Showing the warning message in the Disk Management dialog box.</p></figcaption></figure>

_**Step 6**_

You are back on the **Disk Management** window. Notice that the **Disk 1** status has now changed to **Dynamic**.

Keep the **Disk Management** window open.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-7.jpg?v=24" alt="Figure 1.6 Screenshot of PLABWIN10: Showing the dynamic disk after conversion."><figcaption><p>Figure 1.6 Screenshot of PLABWIN10: Showing the dynamic disk after conversion.</p></figcaption></figure>

#### **Task 2 - Create a Primary Partition** <a href="#cn-m2-96" id="cn-m2-96"></a>

Basic disk partitioning is the most commonly used type of disk partitioning method. Only two types of drives can be created using the basic disk partition method. They are Primary and logical.

The basic file system formats disks using one of the two: Master Boot Record (MBR) or GUID partition table. MBR method makes use of a partition table, which contains a list of locations, where partitions are present. A primary partition, which is marked Active, is the one in which an operating system can be installed.

In this task, you will create a primary partition.

_**Step 1**_

Ensure you are connected to **PLABWIN10** and that the **Disk Management** window is open.

To create a new partition, you require empty space on a hard drive. At present, there is no empty space on any of the hard drives. To create a partition, you need first to create empty space.

Right-click **USB (D:)** in the right pane and then select **Delete volume.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-8.jpg?v=24" alt="Figure 1.7 Screenshot of PLABWIN10: Selecting the Delete Volume option from the context menu."><figcaption><p>Figure 1.7 Screenshot of PLABWIN10: Selecting the Delete Volume option from the context menu.</p></figcaption></figure>

_**Step 2**_

The **Delete simple volume** dialog box is displayed. Click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-9.jpg?v=24" alt="Figure 1.8 Screenshot of PLABWIN10: Showing a warning message in the Delete simple volume dialog box. Yes is selected."><figcaption><p>Figure 1.8 Screenshot of PLABWIN10: Showing a warning message in the Delete simple volume dialog box. Yes is selected.</p></figcaption></figure>

_**Step 3**_

Notice that the **USB (D:)** name is no longer visible. This space is now empty and can be used for creating a partition.

**Disk 1** currently has no partitions, and it is marked as **Unallocated**.

Right-click on **Unallocated** and then select **New Simple Volume** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-10.jpg?v=24" alt="Figure 1.9 Screenshot of PLABWIN10: Selecting the New Simple Volume option from the context menu."><figcaption><p>Figure 1.9 Screenshot of PLABWIN10: Selecting the New Simple Volume option from the context menu.</p></figcaption></figure>

_**Step 4**_

The **New Simple Volume Wizard** is displayed.

On the **Welcome to the New Simple Volume Wizard** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-11.jpg?v=24" alt="Figure 1.10 Screenshot of PLABWIN10: Showing the Welcome page of the New Simple Volume Wizard."><figcaption><p>Figure 1.10 Screenshot of PLABWIN10: Showing the Welcome page of the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 5**_

On the **Specify Volume Size** page, keep the default volume size and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-12.jpg?v=24" alt="Figure 1.11 Screenshot of PLABWIN10: Setting the size of the simple volume on the Specify Volume Size page."><figcaption><p>Figure 1.11 Screenshot of PLABWIN10: Setting the size of the simple volume on the Specify Volume Size page.</p></figcaption></figure>

_**Step 6**_

On the **Assign Drive Letter or Path** page, keep the default selection for the drive letter and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-13.jpg?v=24" alt="Figure 1.12 Screenshot of PLABWIN10: Assigning the drive letter on the Assign Drive Letter or Path page."><figcaption><p>Figure 1.12 Screenshot of PLABWIN10: Assigning the drive letter on the Assign Drive Letter or Path page.</p></figcaption></figure>

_**Step 7**_

On the **Format Partition** page, keep the default options and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-14.jpg?v=24" alt="Figure 1.13 Screenshot of PLABWIN10: Setting the format options on the Format Partition page."><figcaption><p>Figure 1.13 Screenshot of PLABWIN10: Setting the format options on the Format Partition page.</p></figcaption></figure>

_**Step 8**_

On the **Completing the New Simple Volume Wizard** page, click **Finish**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-15.jpg?v=24" alt="Figure 1.14 Screenshot of PLABWIN10: Showing the completion of the New Simple Volume Wizard."><figcaption><p>Figure 1.14 Screenshot of PLABWIN10: Showing the completion of the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 9**_

You are back on the **Disk Management** window. A new primary partition has been created.

Keep the **Disk Management** window open.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-16.jpg?v=24" alt="Figure 1.15 Screenshot of PLABWIN10: Showing the newly created volume in Disk Management."><figcaption><p>Figure 1.15 Screenshot of PLABWIN10: Showing the newly created volume in Disk Management.</p></figcaption></figure>

#### **Task 3 - Create a Primary and Logical Partition** <a href="#cn-m2-142" id="cn-m2-142"></a>

A hard disk can only contain a single extended partition. A single extended partition may contain multiple logical partitions. A logical partition is a sub-division of an extended partition.

Creating an extended partition is possible only on an MBR type of disk.

In this task, you will create a primary partition as well as a logical partition.

_**Note:** Before creating a standard partition, three primary partitions need to be present._

_**Step 1**_

Ensure you are connected to **PLABWIN10** and that the **Disk Management** window is open.

Right-click the **New Volume (D:)** partition in the lower pane and select **Delete Volume**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-17.jpg?v=24" alt="Figure 1.16 Screenshot of PLABWIN10: Selecting the Delete Volume option from the context menu."><figcaption><p>Figure 1.16 Screenshot of PLABWIN10: Selecting the Delete Volume option from the context menu.</p></figcaption></figure>

_**Step 2**_

The **Delete simple volume** dialog box is displayed. Click **Yes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-18.jpg?v=24" alt="Figure 1.17 Screenshot of PLABWIN10: Clicking Yes on the Delete simple volume dialog box."><figcaption><p>Figure 1.17 Screenshot of PLABWIN10: Clicking Yes on the Delete simple volume dialog box.</p></figcaption></figure>

_**Step 3**_

**Disk 1** currently has no partitions, and it is marked as **Unallocated**.

Right-click **Disk 1**, and then select **Convert to MBR Disk** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-19.jpg?v=24" alt="Figure 1.18 Screenshot of PLABWIN10: Selecting the Convert to MBR Disk option from the context menu."><figcaption><p>Figure 1.18 Screenshot of PLABWIN10: Selecting the Convert to MBR Disk option from the context menu.</p></figcaption></figure>

_**Step 4**_

Right-click the **Unallocated** space, and then select **New Simple Volume** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-20.jpg?v=24" alt="Figure 1.19 Screenshot of PLABWIN10: Selecting the New Simple Volume option from the context menu."><figcaption><p>Figure 1.19 Screenshot of PLABWIN10: Selecting the New Simple Volume option from the context menu.</p></figcaption></figure>

_**Step 5**_

The **New Simple Volume Wizard** is displayed.

On the **Welcome to the New Simple Volume Wizard** page, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-21.jpg?v=24" alt="Figure 1.20 Screenshot of PLABWIN10: Showing the welcome page of the New Simple Volume Wizard."><figcaption><p>Figure 1.20 Screenshot of PLABWIN10: Showing the welcome page of the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 6**_

On the **Specify Volume Size** page, enter the following value in the **Simple volume size in MB** text box:

```
500
```

Then, click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-22.jpg?v=24" alt="Figure 1.21 Screenshot of PLABWIN10: Setting the size of the simple volume on the Specify Volume Size page."><figcaption><p>Figure 1.21 Screenshot of PLABWIN10: Setting the size of the simple volume on the Specify Volume Size page.</p></figcaption></figure>

_**Step 7**_

On the **Assign Drive Letter or Path** page, keep the default values and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-23.jpg?v=24" alt="Figure 1.22 Screenshot of PLABWIN10: Assigning the drive letter on the Assign Drive Letter or Path page."><figcaption><p>Figure 1.22 Screenshot of PLABWIN10: Assigning the drive letter on the Assign Drive Letter or Path page.</p></figcaption></figure>

_**Step 8**_

On the **Format Partition** page, keep the default values and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-24.jpg?v=24" alt="Figure 1.23 Screenshot of PLABWIN10: Setting the format options on the Format Partition page."><figcaption><p>Figure 1.23 Screenshot of PLABWIN10: Setting the format options on the Format Partition page.</p></figcaption></figure>

_**Step 9**_

On the **Completing the New Simple Volume Wizard** page, click **Finish**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-25.jpg?v=24" alt="Figure 1.24 Screenshot of PLABWIN10: Showing the completion of the New Simple Volume Wizard."><figcaption><p>Figure 1.24 Screenshot of PLABWIN10: Showing the completion of the New Simple Volume Wizard.</p></figcaption></figure>

_**Step 10**_

Create two more primary partitions. To summarize:

* Right-click the **Unallocated** space, and then select **New Simple Volume** from the context menu.
* Click **Next** when prompted.
* Enter the value **500** in the **Simple volume size in MB** text box.
* Click **Next** when prompted, then **Finish**.

_**Note**: For more detailed instructions, please follow **steps 4-9** in this task._

Then, create one more partition.

Notice that this partition will automatically be marked as **Logical**. The first three partitions are marked as **Primary**.

Keep the **Disk Management** window open.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-26.jpg?v=24" alt="Figure 1.25 Screenshot of PLABWIN10: Showing Disk Management with newly created primary and logical partitions."><figcaption><p>Figure 1.25 Screenshot of PLABWIN10: Showing Disk Management with newly created primary and logical partitions.</p></figcaption></figure>

#### **Task 4 - Convert to MBR or GPT Disk** <a href="#cn-m2-200" id="cn-m2-200"></a>

GPT stands for a GUID Partition Table. A standard called EFI (Extensible Firmware Interface) defines the structure of the partition table.

GPT is a part of the EFI standard. GPT is an enhanced version of the MBR (Master Boot Record) partitioning system.

By using GPT, it is possible to overcome the limitations of an MBR partitioning system.

_**Step 1**_

Ensure you are connected to **PLABWIN10**.

Scroll down the page to right-click **Disk 2**, then select the **Convert to MBR Disk** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-27.jpg?v=24" alt="Figure 1.26 Screenshot of PLABWIN10: Selecting the Convert to MBR Disk from the context menu."><figcaption><p>Figure 1.26 Screenshot of PLABWIN10: Selecting the Convert to MBR Disk from the context menu.</p></figcaption></figure>

_**Step 2**_

Now that the disk is in the MBR format, it can be converted back to the GPT format. Right-click on the **Disk 2** again, then select **Convert to GPT Disk** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-28.jpg?v=24" alt="Figure 1.27 Screenshot of PLABWIN10: Selecting Convert to GPT Disk from the context menu."><figcaption><p>Figure 1.27 Screenshot of PLABWIN10: Selecting Convert to GPT Disk from the context menu.</p></figcaption></figure>

_**Step 3**_

The **Disk 2** is set as GPT disk. Visually, you will not be able to differentiate between the MBR or GPT disk.

Keep the **Disk Management** window open.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m2-c-29.jpg?v=24" alt="Figure 1.28 Screenshot of PLABWIN10: Showing Disk 2 after converting it to GPT disk."><figcaption><p>Figure 1.28 Screenshot of PLABWIN10: Showing Disk 2 after converting it to GPT disk.</p></figcaption></figure>

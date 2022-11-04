# Exercise 1 - Learn About Boot Methods

### **Exercise 1 - Learn About Boot Methods** <a href="#cn-m1-39" id="cn-m1-39"></a>

Booting is the process of powering on the computer and starting the operating system. An operating system is a program, which makes the application programs and the computer hardware work together. The most usual place where you will install an operating system is a hard drive. However, you can also boot a computer with an operating system that runs on a USB drive. You can install an operating system using a hard drive, optical disk, USB drive, or PXE. During the boot process, the device containing the operating system program is loaded in the RAM or computer’s main memory and executed. After execution, the operating system becomes functional and takes over control of the machine.



#### **Task 1 - Set up a Boot Device** <a href="#cn-m1-50" id="cn-m1-50"></a>

Operating system files can be loaded from an external storage device. The device could be an optical disk or a USB drive. The methods of installing an operating system from these devices are similar.

To load an operating system from a DVD, perform the following steps:

_**Step 1**_

Ensure all the required device are powered on and connect to **PLABWIN10**. Close any open windows.

Click the **Hyper-V Manager** icon on the taskbar.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-2.jpg?v=18" alt="Figure 1.1 Screenshot of PLABWIN10: Clicking the Hyper-V Manager icon in the taskbar."><figcaption><p>Figure 1.1 Screenshot of PLABWIN10: Clicking the Hyper-V Manager icon in the taskbar.</p></figcaption></figure>

_**Step 2**_

The **Hyper-V Manager** window is displayed.

In the central pane, right-click **PLABWIN101** and select **Settings** from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-3.jpg?v=18" alt="Figure 1.2 Screenshot of PLABWIN10: Right-clicking the PLABWIN101 virtual machine and selecting Settings from the context menu."><figcaption><p>Figure 1.2 Screenshot of PLABWIN10: Right-clicking the PLABWIN101 virtual machine and selecting Settings from the context menu.</p></figcaption></figure>

_**Step 3**_

The **Settings for PLABWIN101 on PLABWIN10** dialog box is displayed.

In the **Hardware** pane, select **BIOS**. The BIOS panel is displayed in the right pane.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-4.jpg?v=18" alt="Figure 1.3 Screenshot of PLABWIN10: Displaying the BIOS boot menu of the virtual machine."><figcaption><p>Figure 1.3 Screenshot of PLABWIN10: Displaying the BIOS boot menu of the virtual machine.</p></figcaption></figure>

_**Step 4**_

Under the **Startup order** list box, a list of devices is displayed. Any of these devices can be used for booting purpose.

Devices are checked in this order for the availability of an operating system. For this, the order can be chosen.

Select **IDE** in the list box and click the **Move Up** button.

This will set IDE as the first choice for booting.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-5.jpg?v=18" alt="Figure 1.4 Screenshot of PLABWIN10: Selecting IDE and moving it up as the boot device."><figcaption><p>Figure 1.4 Screenshot of PLABWIN10: Selecting IDE and moving it up as the boot device.</p></figcaption></figure>

_**Step 5**_

IDE is now the preferred boot device. The system will first check IDE for a bootable operating system and then move to the CD.

Select the **CD** and click the **Move Up** button.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-6.jpg?v=18" alt="Figure 1.5 Screenshot of PLABWIN10: Selecting CD and moving it up as the boot device."><figcaption><p>Figure 1.5 Screenshot of PLABWIN10: Selecting CD and moving it up as the boot device.</p></figcaption></figure>

_**Step 6**_

CD is now the first device in the boot order.

Click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m1-c-7.jpg?v=18" alt="Figure 1.6 Screenshot of PLABWIN10: Clicking the OK button on the Settings for PLABWIN101 on PLABWIN10 window."><figcaption><p>Figure 1.6 Screenshot of PLABWIN10: Clicking the OK button on the Settings for PLABWIN101 on PLABWIN10 window.</p></figcaption></figure>

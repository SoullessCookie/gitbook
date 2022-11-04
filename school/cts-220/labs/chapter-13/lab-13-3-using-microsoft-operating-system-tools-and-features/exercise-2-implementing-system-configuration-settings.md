# Exercise 2 - Implementing System Configuration Settings

### **Exercise 2 - Implementing System Configuration Settings** <a href="#cn-m5-391" id="cn-m5-391"></a>

**System Configuration** is a Windows tool that helps in configuring settings, such as the boot options for the machine, services to be enabled/disabled for a login, and programs to run at the startup of the machine. If you have multiple operating systems installed, you can configure the system to boot with a specific operating system by default. Moreover, you can also make settings for other Windows tools, such as **Action Center**.



#### **Task 1 - Specify the Startup Type for Computer** <a href="#cn-m5-405" id="cn-m5-405"></a>

The **System Configuration** console has the following tabs - **General**, **Boot**, **Services**, **Startup**, and **Tools**. As the names suggest, each tab provides options for configuring the relevant settings.

The **General** tab provides the following options for the Windows startup:

* **Normal startup** - loading all the device drivers and services
* **Diagnostic startup** - loading only basic devices and services
* **Selective startup** - you select the services and items to load

In this task, you will specify the **Diagnostic startup** for the computer.

_**Step 1**_

Ensure **PLABWIN10** is powered on.

In the **Type here to search** textbox in the taskbar and type the following:

```
System Configuration
```

Under **Best Match** section, select **System Configuration**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-51.jpg?v=29" alt="Figure 2.1 Screenshot of PLABWIN10: Selecting System Configuration from the search results."><figcaption><p>Figure 2.1 Screenshot of PLABWIN10: Selecting System Configuration from the search results.</p></figcaption></figure>

_**Step 2**_

The **System Configuration** dialog box is displayed.

Notice that the **General** tab is displayed by default.

On the **General** tab, select the **Diagnostic Startup - load basic devices and services only** option.

Click **Apply**.

_**Note:** Please be aware that if the setting does not apply, please continue. You do not apply any of the changes below as they would require a system reboot which is not needed for this module._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-52.jpg?v=29" alt="Figure 2.2 Screenshot of PLABWIN10: Showing the General tab on the System Configuration dialog box and selecting the Diagnostic startup."><figcaption><p>Figure 2.2 Screenshot of PLABWIN10: Showing the General tab on the System Configuration dialog box and selecting the Diagnostic startup.</p></figcaption></figure>

#### **Task 2 - Set the Timeout Period on the Boot Tab** <a href="#cn-m5-430" id="cn-m5-430"></a>

Options on the **Boot** tab allow you to specify which operating system should load, in-case you have multiple. It also allows you to make choices, such as Safe boot, which is mainly used for troubleshooting purposes and loads only the necessary services and system programs.

In this task, you will specify the timeout period on the **Boot** tab.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **System Configuration** dialog box is displayed.

Click the **Boot** tab.

Set **Timeout** period as 20 seconds.

Press **Apply**.

With this setting, the system waits 20 seconds for a user to make operating system selection; otherwise, it will proceed with the default specification.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-53.jpg?v=29" alt="Figure 2.3 Screenshot of PLABWIN10: Showing the Boot tab on the System Configuration dialog box with the required configuration changes."><figcaption><p>Figure 2.3 Screenshot of PLABWIN10: Showing the Boot tab on the System Configuration dialog box with the required configuration changes.</p></figcaption></figure>

#### **Task 3 - Disable a Service on the Services Tab** <a href="#cn-m5-443" id="cn-m5-443"></a>

The **Services** tab on the **System Configuration** dialog box lists all the services present on the computer system. Along with service name, the tab also mentions the **Manufacturer**, **Status**, and **Date Disabled** for each service.

In this task, you will disable the **Microsoft Audio** service on the computer.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **System Configuration** dialog box is displayed.

Click the **Services** tab.

Notice that either you can enable or disable all services. However, you cannot enable or disable a single service.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-54.jpg?v=29" alt="Figure 2.4 Screenshot of PLABWIN10: Showing the Services tab on the System Configuration dialog box."><figcaption><p>Figure 2.4 Screenshot of PLABWIN10: Showing the Services tab on the System Configuration dialog box.</p></figcaption></figure>

_**Step 2**_

Select Windows Audio. Notice that **Disable All** button is now enabled.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-55.jpg?v=29" alt="Figure 2.5 Screenshot of PLABWIN10: Selecting a service and then showing the Disable All button highlighted."><figcaption><p>Figure 2.5 Screenshot of PLABWIN10: Selecting a service and then showing the Disable All button highlighted.</p></figcaption></figure>

_**Step 3**_

Select **Hide all Microsoft services**. Notice now the **Services** tab does not have any service listed.

Click **Apply**.

_**Note:** There may be a service or some services still listed, please continue to the next task._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-56.jpg?v=29" alt="Figure 2.6 Screenshot of PLABWIN10: Hiding all the Microsoft services."><figcaption><p>Figure 2.6 Screenshot of PLABWIN10: Hiding all the Microsoft services.</p></figcaption></figure>

#### **Task 4 - Enable Microsoft OneDrive as a Startup Service** <a href="#cn-m5-463" id="cn-m5-463"></a>

The **Startup** tab lists the startup items, along with information such as the publisher of the item, status, and startup impact. On the **Startup** tab, you can enable/disable individual/multiple start-up items.

In this task, you will enable the **Microsoft OneDrive** to start-up with the computer.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **System Configuration** dialog box is displayed.

Click the **Startup** tab.

Click the **Open Task Manager** link.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-57.jpg?v=29" alt="Figure 2.7 Screenshot of PLABWIN10: Clicking the Open Task Manager link on the Startup tab of the System Configuration dialog box."><figcaption><p>Figure 2.7 Screenshot of PLABWIN10: Clicking the Open Task Manager link on the Startup tab of the System Configuration dialog box.</p></figcaption></figure>

_**Step 2**_

The **Task Manager** dialog box is displayed. By default, the **Startup** tab is selected. On the **Startup** tab, select the **Microsoft OneDrive** option and click **Enable**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-58.jpg?v=29" alt="Figure 2.8 Screenshot of PLABWIN10: Showing the Startup tab on the Task Manager dialog box with the required selection performed and the Enable button highlighted."><figcaption><p>Figure 2.8 Screenshot of PLABWIN10: Showing the Startup tab on the Task Manager dialog box with the required selection performed and the Enable button highlighted.</p></figcaption></figure>

_**Step 3**_

Notice that the **Status** of the **Microsoft OneDrive** service is now changed to **Enabled**. This specifies the **Microsoft OneDrive** as a startup service.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-59.jpg?v=29" alt="Figure 2.9 Screenshot of PLABWIN10: Showing the enabled Microsoft OneDrive service."><figcaption><p>Figure 2.9 Screenshot of PLABWIN10: Showing the enabled Microsoft OneDrive service.</p></figcaption></figure>

Close the **Task Manager** dialog box.

_**Step 4**_

You are back on the **Startup** tab of the **System Configuration** dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-60.jpg?v=29" alt="Figure 2.10 Screenshot of PLABWIN10: Displaying the Startup tab on the Task Manager."><figcaption><p>Figure 2.10 Screenshot of PLABWIN10: Displaying the Startup tab on the Task Manager.</p></figcaption></figure>

#### **Task 5 - Launch a Tool from the Tools Tab** <a href="#cn-m5-490" id="cn-m5-490"></a>

The **Tools** tab lists the available tools and their description. You can select and launch a tool from here.

In this task, you will access the **About Windows** information on the **Tools** tab.

_**Step 1**_

Ensure that **PLABWIN10** is running and the **System Configuration** dialog box is displayed.

Click the **Tools** tab.

Select the **About Windows** option and click **Launch**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-61.jpg?v=29" alt="Figure 2.11 Screenshot of PLABWIN10: Launching the About Windows dialog box."><figcaption><p>Figure 2.11 Screenshot of PLABWIN10: Launching the About Windows dialog box.</p></figcaption></figure>

_**Step 2**_

The **About Windows** window is displayed.

View the information and click **OK** to exit the **About Windows** dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-62.jpg?v=29" alt="Figure 2.12 Screenshot of PLABWIN10: Showing the About Windows dialog box and showing the OK button highlighted."><figcaption><p>Figure 2.12 Screenshot of PLABWIN10: Showing the About Windows dialog box and showing the OK button highlighted.</p></figcaption></figure>

_**Step 3**_

Back on the **System Configuration** dialog box, click **OK** to save the changes and exit.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-63.jpg?v=29" alt="Figure 2.13 Screenshot of PLABWIN10: Showing the OK button highlighted on the System Configuration dialog box."><figcaption><p>Figure 2.13 Screenshot of PLABWIN10: Showing the OK button highlighted on the System Configuration dialog box.</p></figcaption></figure>

_**Step 4**_

The **System Configuration** dialog box is displayed. You can apply the changes immediately by restarting the system or exit without restarting. For this task, click **Exit without restart**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-64.jpg?v=29" alt="Figure 2.14 Screenshot of PLABWIN10: Showing the System Configuration dialog box with the Exit without restart button highlighted."><figcaption><p>Figure 2.14 Screenshot of PLABWIN10: Showing the System Configuration dialog box with the Exit without restart button highlighted.</p></figcaption></figure>

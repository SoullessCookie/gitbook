# Exercise 3 - Using the Task Manager



### **Exercise 3 - Using the Task Manager** <a href="#cn-m5-518" id="cn-m5-518"></a>

**Task Manager** is a Windows tool that enables you to track, monitor, and troubleshoot the system performance at levels starting from the OS level right up to the individual application level.

Features of the **Task Manager** are organized into the following tabs:

* Processes
* Performance
* App History
* Startup
* Users
* Details
* Services



#### **Task 1 -End a Task on the Processes Tab** <a href="#cn-m5-539" id="cn-m5-539"></a>

The **Processes** tab is the first tab on the **Task Manager** console. This tab lists the processes and applications running on the system while tracking the number of resources - **CPU**, **Memory**, **Disk**, and **Network** - that each process/application is using. There will be scenarios in which an application, such as Google Chrome or Microsoft Word, consume a large amount of memory or CPU. In that case, you can use the Processes tab to terminate the processes specific to these applications. In this task, you will stop the execution of the **Antimalware Service Executable** process.

_**Step 1**_

Ensure **PLABWIN10** is running and the desktop is displayed. Right-click the **taskbar** and select Task Manager from the context menu.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-66.jpg?v=29" alt="Figure 3.1 Screenshot of PLABWIN10: Selecting Task Manager from the context menu of Windows taskbar."><figcaption><p>Figure 3.1 Screenshot of PLABWIN10: Selecting Task Manager from the context menu of Windows taskbar.</p></figcaption></figure>

_**Step 2**_

**Task Manager** is displayed.

Notice that the **Processes** tab is displayed by default.

On the **Processes** tab, the list of running processes - along with the resource-usage by each - is organized into two sections - **Applications** and **Background processes**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-67.jpg?v=29" alt="Figure 3.2 Screenshot of PLABWIN10: Showing the Processes tab on the Task Manager window."><figcaption><p>Figure 3.2 Screenshot of PLABWIN10: Showing the Processes tab on the Task Manager window.</p></figcaption></figure>

_**Step 3**_

For this task, select the **Antimalware Service Executable** process, then click **End task**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-68.jpg?v=29" alt="Figure 3.3 Screenshot of PLABWIN10: Selecting the Antimalware Service Executable process, then clicking End task."><figcaption><p>Figure 3.3 Screenshot of PLABWIN10: Selecting the Antimalware Service Executable process, then clicking End task.</p></figcaption></figure>

_**Step 4**_

Since this is a system-controlled process, it cannot be terminated. Notice that the **Unable to terminate process** dialog box is displayed. Click **OK** to close this dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-69.jpg?v=29" alt="Figure 3.4 Screenshot of PLABWIN10: Showing the Access is denied message."><figcaption><p>Figure 3.4 Screenshot of PLABWIN10: Showing the Access is denied message.</p></figcaption></figure>

_**Step 5**_

Select **Microsoft Edge** and click **End task**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-70.jpg?v=29" alt="Figure 3.5 Screenshot of PLABWIN10: Selecting Microsoft Edge and clicking End task."><figcaption><p>Figure 3.5 Screenshot of PLABWIN10: Selecting Microsoft Edge and clicking End task.</p></figcaption></figure>

_**Step 6**_

Notice that **Microsoft Edge** no longer appears in the list. It has been terminated.

Keep the **Task Manager** open for the next task.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-71.jpg?v=29" alt="Figure 3.6 Screenshot of PLABWIN10: Showing the updated task list without Microsoft Edge."><figcaption><p>Figure 3.6 Screenshot of PLABWIN10: Showing the updated task list without Microsoft Edge.</p></figcaption></figure>

#### **Task 2 - Explore the Performance Tab** <a href="#cn-m5-568" id="cn-m5-568"></a>

The **Performance** tab on the **Task Manager** monitors and tracks the system parameters - **CPU**, **Memory**, **Disk**, and **Ethernet**. The performance-history is traced as a graph to refer to during performance analysis or troubleshooting. In addition, statistics relevant to each feature appear on the tab.

In this task, you will explore the Performance tab on the Task Manager console.

_**Step 1**_

Ensure **PLABWIN10** is running and the **Task Manager** console is displayed.

Click the **Performance** tab.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-72.jpg?v=29" alt="Figure 3.7 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the CPU parameter."><figcaption><p>Figure 3.7 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the CPU parameter.</p></figcaption></figure>

_**Step 2**_

Notice that the performance graph and the relevant statistics for the **CPU** parameter are displayed by default. This tab, depending on what you have selected, for example, CPU, displays the configuration statistics. It displays statistics, such as virtual processors, sockets, utilization, processes, threats, handles, and the processor speed. It also provides the uptime for the processor.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-73.jpg?v=29" alt="Figure 3.8 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the CPU parameter"><figcaption><p>Figure 3.8 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the CPU parameter</p></figcaption></figure>

_**Step 3**_

Select **Memory**. Just like CPU, memory statistics are being displayed. The graph displays a visual of the memory being used.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-74.jpg?v=29" alt="Figure 3.9 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the memory parameter."><figcaption><p>Figure 3.9 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the memory parameter.</p></figcaption></figure>

_**Step 4**_

Select **Disk 0**. The disk statistics are displayed. Notice that there are three disks being displayed. When you have more than one disk, it is marked as **Disk 0**, **Disk 1**, and so on.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-75.jpg?v=29" alt="Figure 3.10 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the disk parameter"><figcaption><p>Figure 3.10 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the disk parameter</p></figcaption></figure>

_**Step 5**_

Select **Ethernet. Ethernet** is another option on the **Performance** tab that you might access often to analyze the performance history of the local system.

Notice that the **Ethernet** option also lists other relevant details such as adapter name, connection type, IP addresses, and data speeds.

_**Note**: One Ethernet option is listed on the Performance tab for each Ethernet cable connected to the machine._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-76.jpg?v=29" alt="Figure 3.11 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the Ethernet parameter"><figcaption><p>Figure 3.11 Screenshot of PLABWIN10: Showing the Performance tab on the Task Manager and showing the relevant statistics for the Ethernet parameter</p></figcaption></figure>

#### **Task 3 - Disconnect a User on the Users Tab** <a href="#cn-m5-594" id="cn-m5-594"></a>

The **Users** tab on the **Task Manager** console lists the number of users on the machine, along with the details, such as the status of the user and system-resource consumption. You can use this information to monitor and track the resource-usage for a user and if required, disconnect the user. In this task, you will disconnect a listed user.

_**Step 1**_

Ensure **PLABWIN10** is running and the **Task Manager** console is displayed.

Click the **Users** tab. Notice that there is only one user connected.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-77.jpg?v=29" alt="Figure 3.12 Screenshot of PLABWIN10: Showing the Users tab on the Task Manager."><figcaption><p>Figure 3.12 Screenshot of PLABWIN10: Showing the Users tab on the Task Manager.</p></figcaption></figure>

_**Step 2**_

To disconnect **Administrator**, select it and click **Disconnect**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-78.jpg?v=29" alt="Figure 3.13 Screenshot of PLABWIN10: Selecting Administrator and then clicking the Disconnect button."><figcaption><p>Figure 3.13 Screenshot of PLABWIN10: Selecting Administrator and then clicking the Disconnect button.</p></figcaption></figure>

_**Step 3**_

The **Task Manager** dialog box is displayed. To confirm the disconnection, click **Disconnect user**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-79.jpg?v=29" alt="Figure 3.14 Screenshot of PLABWIN10: Confirming the disconnection by clicking the Disconnect user button."><figcaption><p>Figure 3.14 Screenshot of PLABWIN10: Confirming the disconnection by clicking the Disconnect user button.</p></figcaption></figure>

_**Step 4**_

Notice that the session is disconnected. You have forcefully disconnected yourself.

_**Note:** Similarly, you can view and explore the other tabs on the Task Manager console._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-80.jpg?v=29" alt="Figure 3.15 Screenshot of PLABWIN10: Showing the disconnected user and the session."><figcaption><p>Figure 3.15 Screenshot of PLABWIN10: Showing the disconnected user and the session.</p></figcaption></figure>

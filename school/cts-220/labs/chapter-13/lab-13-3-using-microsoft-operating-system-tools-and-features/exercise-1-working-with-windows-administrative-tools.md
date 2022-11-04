# Exercise 1 - Working with Windows Administrative Tools



### **Exercise 1 - Working with Windows Administrative Tools** <a href="#cn-m5-60" id="cn-m5-60"></a>

Administrative tools are a collection of computer management services that help to perform regular maintenance tasks, such as disk defragmentation, disk clean-up, and running system memory diagnostics. These tools also help manage the system by defining the security policy for Windows and other devices running on the system. Administrative tools are available on the **Start** screen or even as a part of the **Control Panel**.



#### **Task 1 - Access Computer Management Tools** <a href="#cn-m5-78" id="cn-m5-78"></a>

Computer management services enable you to manage system tools, storage, services, and applications of your local or remote system. Moreover, by using these tools you can automate some of the routine system management tasks. **Computer Management** tools are available as a part of the **Administrative tools**.

In this task, you will access the **Computer Management** tools.

_**Step 1**_

Ensure **PLABWIN10** is powered on and connected.

The desktop is displayed.

In the **Type here to search** textbox in the taskbar, type the following:

```
Administrative Tools  
```

Under **Best Match** section, select **Administrative Tools**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-2.jpg?v=29" alt="Figure 1.1 Screenshot of PLABWIN10: Selecting Administrative Tools from the search results."><figcaption><p>Figure 1.1 Screenshot of PLABWIN10: Selecting Administrative Tools from the search results.</p></figcaption></figure>

_**Step 2**_

In the **Administrative Tools** window, double-click **Computer Management**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-3.jpg?v=29" alt="Figure 1.2 Screenshot of PLABWIN10: Double-clicking Computer Management in the Administrative Tools window."><figcaption><p>Figure 1.2 Screenshot of PLABWIN10: Double-clicking Computer Management in the Administrative Tools window.</p></figcaption></figure>

_**Step 3**_

The **Computer Management** console is displayed.

Several tools and utilities are listed here under three different sections:

* **System Tools**: This contains tools, such as Event Viewer, Shared Folders, Local Users and Groups.
* **Storage**: This contains Disk Management, which allows you to create, delete, and modify partitions on your local system.
* **Services and Applications**: This contains Services and WMI Control, which is Windows Management Instrumentation.

It is important to note that all these tools are available individually. For example, you can manage services from the Services console or from the **Services** node in **Computer Management**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-4.jpg?v=29" alt="Figure 1.3 Screenshot of PLABWIN10: Displaying the Computer Management window with its tools."><figcaption><p>Figure 1.3 Screenshot of PLABWIN10: Displaying the Computer Management window with its tools.</p></figcaption></figure>

_**Step 4**_

Expand the **Services and Applications** node in the left pane and select **Services**.

The Windows services are displayed. Each service must have a status. For example, a service can be running or stopped. The services that are running are marked with **Running** status. Stopped services do not have any status displayed.

Close the **Computer Management** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-5.jpg?v=29" alt="Figure 1.4 Screenshot of PLABWIN10: Using the Services node in the Computer Management window."><figcaption><p>Figure 1.4 Screenshot of PLABWIN10: Using the Services node in the Computer Management window.</p></figcaption></figure>

#### **Task 2 - Configure Local Security Policy** <a href="#cn-m5-108" id="cn-m5-108"></a>

Local security policy configures the security settings of your local machine; thereby allowing you to make your device more secure, taking care of possible threats. For example, by using these policies you can configure the system firewall, set application and software control policies, enforce passwords, specify trusted domains, configure access rights, define account privileges, and schedule security auditing.

These settings can be broadly categorized into three types - user-related settings, system-related settings, and security-related settings.

In this task, you will modify the password settings on the system.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

On the **Administrative Tools** window, double-click **Local Security Policy**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-6.jpg?v=29" alt="Figure 1.5 Screenshot of PLABWIN10: Double-clicking Local Security Policy."><figcaption><p>Figure 1.5 Screenshot of PLABWIN10: Double-clicking Local Security Policy.</p></figcaption></figure>

_**Step 2**_

On the **Local Security Policy** window, expand **Account Policies** and then select **Password Policy** in the left pane.

Notice that the right pane displays the password related policies.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-7.jpg?v=29" alt="Figure 1.6 Screenshot of PLABWIN10: Displaying policies listed under Password Policy."><figcaption><p>Figure 1.6 Screenshot of PLABWIN10: Displaying policies listed under Password Policy.</p></figcaption></figure>

_**Step 3**_

On the details pane at the right, double-click the **Maximum password age** policy.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-8.jpg?v=29" alt="Figure 1.7 Screenshot of PLABWIN10: Double-clicking the Maximum password age policy"><figcaption><p>Figure 1.7 Screenshot of PLABWIN10: Double-clicking the Maximum password age policy</p></figcaption></figure>

_**Step 4**_

The **Maximum password age Properties** dialog box is displayed.

Notice that the value is non-editable. This is because this value is being inherited from the domain controller. By default, the domain members inherit password policy values from the domain controller.

Click **OK**.

_**Note**: By default, 42 days is the default domain policy setting for maximum password age._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-9.jpg?v=29" alt="Figure 1.8 Screenshot of PLABWIN10: Closing the Maximum password age Properties dialog box."><figcaption><p>Figure 1.8 Screenshot of PLABWIN10: Closing the Maximum password age Properties dialog box.</p></figcaption></figure>

_**Step 5**_

Let’s look at some of the policies that can be configured locally even if the system is a domain member.

Expand the **Local Policies** node in the left pane and select **Audit Policy**. Notice that the right pane displays audit related policies.

In the right pane, double-click the **Audit account logon events** policy.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-10.jpg?v=29" alt="Figure 1.9 Screenshot of PLABWIN10: Double-clicking the Audit Account logon events policy."><figcaption><p>Figure 1.9 Screenshot of PLABWIN10: Double-clicking the Audit Account logon events policy.</p></figcaption></figure>

_**Step 6**_

In the **Audit account logon events Properties** dialog box, select **Failure** and then click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-11.jpg?v=29" alt="Figure 1.10 Screenshot of PLABWIN10: Selecting Failure in the Audit account logon events Properties dialog box."><figcaption><p>Figure 1.10 Screenshot of PLABWIN10: Selecting Failure in the Audit account logon events Properties dialog box.</p></figcaption></figure>

_**Step 7**_

Notice that the status for **Audit account logon events** policy has changed to **Failure**.

_**Note:** If time permits, you may want to review some of the policies._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-12.jpg?v=29" alt="Figure 1.11 Screenshot of PLABWIN10: Showing Failure as the status for Audit account logon events policy."><figcaption><p>Figure 1.11 Screenshot of PLABWIN10: Showing Failure as the status for Audit account logon events policy.</p></figcaption></figure>

#### **Task 3 - Create a Task on the Task Scheduler** <a href="#cn-m5-148" id="cn-m5-148"></a>

The task scheduler allows you to automate the schedule to start/run/stop a task. For example, you can specify the applications that shall start when a specific event occurs. The specified application will start and run as specified in the setting. In addition, you can view the already running tasks, and you can also import a task.

In the following steps, you will create a basic task.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

Double-click **Task Scheduler**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-13.jpg?v=29" alt="Figure 1.12 Screenshot of PLABWIN10: Double-clicking Task Schedule in Administrative Tools window."><figcaption><p>Figure 1.12 Screenshot of PLABWIN10: Double-clicking Task Schedule in Administrative Tools window.</p></figcaption></figure>

_**Step 2**_

On the **Task Scheduler** console displayed, click the **Create Basic Task** option in the right pane.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-14.jpg?v=29" alt="Figure 1.13 Screenshot of PLABWIN10: Clicking the Create Basic Task option"><figcaption><p>Figure 1.13 Screenshot of PLABWIN10: Clicking the Create Basic Task option</p></figcaption></figure>

_**Step 3**_

The **Create Basic Task Wizard** is displayed.

On the **Create a Basic Task** page, in the **Name** section, type:

```
Starting Component Services
```

In the **Description**, type:

```
Automatically starts the component services when the system boots.
```

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-15.jpg?v=29" alt="Figure 1.14 Screenshot of PLABWIN10: Adding value in the fields on the Create a Basic Task page."><figcaption><p>Figure 1.14 Screenshot of PLABWIN10: Adding value in the fields on the Create a Basic Task page.</p></figcaption></figure>

_**Step 4**_

On the **Task Trigger** page, under the **When do you want the task to start?** question, select the **When the computer starts** option, and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-16.jpg?v=29" alt="Figure 1.15 Screenshot of PLABWIN10: Selecting the task start on the Task Trigger page."><figcaption><p>Figure 1.15 Screenshot of PLABWIN10: Selecting the task start on the Task Trigger page.</p></figcaption></figure>

_**Step 5**_

On the **Action** page, ensure that the **Start a Program** option is selected, and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-17.jpg?v=29" alt="Figure 1.16 Screenshot of PLABWIN10: Keeping the Start a program selected and clicking Next."><figcaption><p>Figure 1.16 Screenshot of PLABWIN10: Keeping the Start a program selected and clicking Next.</p></figcaption></figure>

_**Step 6**_

On the **Start a Program** page, click **Browse** to select the required program.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-18.jpg?v=29" alt="Figure 1.17 Screenshot of PLABWIN10: Clicking Browse on the Start a Program page."><figcaption><p>Figure 1.17 Screenshot of PLABWIN10: Clicking Browse on the Start a Program page.</p></figcaption></figure>

_**Step 7**_

The **Open** dialog box is displayed.

Select the **Component Services** from the available options.

Click **Open.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-19.jpg?v=29" alt="Figure 1.18 Screenshot of PLABWIN10: Selecting Component Services in the Open dialog box and then clicking Open."><figcaption><p>Figure 1.18 Screenshot of PLABWIN10: Selecting Component Services in the Open dialog box and then clicking Open.</p></figcaption></figure>

_**Step 8**_

Back in the **Start a Program** page, notice that the selected program is now listed for a scheduled startup.

Click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-20.jpg?v=29" alt="Figure 1.19 Screenshot of PLABWIN10: Clicking Next after adding a program on the Start a Program page."><figcaption><p>Figure 1.19 Screenshot of PLABWIN10: Clicking Next after adding a program on the Start a Program page.</p></figcaption></figure>

_**Step 9**_

The **Summary** page is displayed listing a summary of the specifications for the task scheduling activity.

Click **Finish** to create a task in the **Windows scheduler**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-21.jpg?v=29" alt="Figure 1.20 Screenshot of PLABWIN10: Showing the Summary page on the Create Basic Task Wizard and showing the Finish button highlighted."><figcaption><p>Figure 1.20 Screenshot of PLABWIN10: Showing the Summary page on the Create Basic Task Wizard and showing the Finish button highlighted.</p></figcaption></figure>

_**Step 10**_

You are back on the **Task Scheduler** window.

Tasks are stored as files in the **Task Scheduler Library**.

To view the newly created task, select the **Task Scheduler Library** node in the left pane

All the tasks are listed in the middle pane. Notice that the Starting Component Services task is also listed.

Close the **Task Scheduler** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-22.jpg?v=29" alt="Figure 1.21 Screenshot of PLABWIN10: Showing the newly created task listed on the middle pane of the Task Scheduler console."><figcaption><p>Figure 1.21 Screenshot of PLABWIN10: Showing the newly created task listed on the middle pane of the Task Scheduler console.</p></figcaption></figure>

#### **Task 4 - Explore Print Management Properties** <a href="#cn-m5-205" id="cn-m5-205"></a>

The print management option of **Administrative Tools** allows you to view the overall status of various printers associated with the computer system. It allows you to access printer properties, configure print-related settings, and view print server-related information. In addition, it allows you to view information such as which printer(s) is ready/not ready, which printer(s) is currently assigned a job(s), and the length of the print job queue.

In this task, you will observe the properties of one of the printers configured on the system.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

Double-click **Print Management**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-23.jpg?v=29" alt="Figure 1.22 Screenshot of PLABWIN10: Double-clicking Print Management in the Administrative Tools window."><figcaption><p>Figure 1.22 Screenshot of PLABWIN10: Double-clicking Print Management in the Administrative Tools window.</p></figcaption></figure>

_**Step 2**_

The **Print Management** console is displayed.

Under the **Custom Filters** section, select **All Printers** in the left pane.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-24.jpg?v=29" alt="Figure 1.23 Screenshot of PLABWIN10: Showing the Print Management window with the All Printers node selected in the left pane."><figcaption><p>Figure 1.23 Screenshot of PLABWIN10: Showing the Print Management window with the All Printers node selected in the left pane.</p></figcaption></figure>

_**Step 3**_

All the printers configured on the system are now listed on the middle pane of the **Print Management** console.

Right-click **Fax** and select **Properties**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-25.jpg?v=29" alt="Figure 1.24 Screenshot of PLABWIN10: Showing the Context menu after right-clicking Fax and then selecting Properties."><figcaption><p>Figure 1.24 Screenshot of PLABWIN10: Showing the Context menu after right-clicking Fax and then selecting Properties.</p></figcaption></figure>

_**Step 4**_

The **Fax Properties** dialog box is displayed. Notice that there are four tabs:

* **General**: Allows you to configure page layout settings.
* **Sharing**: Displays the sharing options. For Fax, even though the tab is listed, you cannot share a Fax.
* **Color Management**: Allows you to configure the color related settings.
* **Security**: Allows you to configure permissions.

Click **Preferences**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-26.jpg?v=29" alt="Figure 1.25 Screenshot of PLABWIN10: Showing the Fax Properties dialog box and showing the Preferences button highlighted."><figcaption><p>Figure 1.25 Screenshot of PLABWIN10: Showing the Fax Properties dialog box and showing the Preferences button highlighted.</p></figcaption></figure>

_**Step 5**_

The **Fax Printing Properties** dialog box is displayed.

From the **Paper size** drop-down list, select **A4 Small** and click **OK**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-27.jpg?v=29" alt="Figure 1.26 Screenshot of PLABWIN10: Showing the Fax Printing Preferences dialog box and showing the OK button highlighted."><figcaption><p>Figure 1.26 Screenshot of PLABWIN10: Showing the Fax Printing Preferences dialog box and showing the OK button highlighted.</p></figcaption></figure>

_**Step 6**_

Back on the **Fax Properties** dialog box, click **OK**.

Close the **Print Management** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-28.jpg?v=29" alt="Figure 1.27 Screenshot of PLABWIN10: Showing the OK button highlighted on the Fax Properties dialog box."><figcaption><p>Figure 1.27 Screenshot of PLABWIN10: Showing the OK button highlighted on the Fax Properties dialog box.</p></figcaption></figure>

#### **Task 5 - Configure Windows Memory Diagnostics** <a href="#cn-m5-242" id="cn-m5-242"></a>

**Windows Memory Diagnostics** is a Windows tool that can scan the system memory at the booting time. This scan is more thorough than a similar scan performed by the BIOS system. Therefore, a scan by the **Windows Memory Diagnostics** tool is more reliable and is able to identify more threats than the BIOS scan.

In this task, you will configure the **Windows Memory Scan** to scan the memory whenever the computer starts-up next.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

Select the **Windows Memory Diagnostic** option.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-29.jpg?v=29" alt="Figure 1.28 Screenshot of PLABWIN10: Double-clicking Windows Memory Diagnostic in the Administrative Tools window."><figcaption><p>Figure 1.28 Screenshot of PLABWIN10: Double-clicking Windows Memory Diagnostic in the Administrative Tools window.</p></figcaption></figure>

_**Step 2**_

The **Check your computer for memory problems** dialog box is displayed.

Click the **Check for problems the next time I start my computer** option.

A scan will be performed when the computer system starts-up the next time.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-30.jpg?v=29" alt="Figure 1.29 Screenshot of PLABWIN10: Clicking the Check for problems the next time I start my computer option in the Windows Memory Diagnostic dialog box."><figcaption><p>Figure 1.29 Screenshot of PLABWIN10: Clicking the Check for problems the next time I start my computer option in the Windows Memory Diagnostic dialog box.</p></figcaption></figure>

_**Step 3**_

**The memory test was scheduled successfully** dialog box is displayed confirming the memory diagnostic setup.

Click **Close** to exit the dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-31.jpg?v=29" alt="Figure 1.30 Screenshot of PLABWIN10: Displaying the Windows Memory Diagnostic dialog box with the Close button highlighted."><figcaption><p>Figure 1.30 Screenshot of PLABWIN10: Displaying the Windows Memory Diagnostic dialog box with the Close button highlighted.</p></figcaption></figure>

#### **Task 6 - Explore Component Services** <a href="#cn-m5-261" id="cn-m5-261"></a>

**Component Services** tool is a part of the **Administrative Tools** console. **Component services** enable you to configure and administer various COM/DCOM applications and components on the computer.

_**Note:** To understand COM/DCOM further, refer to the following URL: https://bit.ly/2RXLFDc_

In this task, you will explore the **Component Services** configuration on the system.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

Double-click **Component Services**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-32.jpg?v=29" alt="Figure 1.31 Screenshot of PLABWIN10: Double-clicking Component Services in the Administrative Tools window."><figcaption><p>Figure 1.31 Screenshot of PLABWIN10: Double-clicking Component Services in the Administrative Tools window.</p></figcaption></figure>

_**Step 2**_

The **Component Services** window is displayed.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-33.jpg?v=29" alt="Figure 1.32 Screenshot of PLABWIN10: Showing the Component Services console."><figcaption><p>Figure 1.32 Screenshot of PLABWIN10: Showing the Component Services console.</p></figcaption></figure>

_**Step 3**_

On the **Console Root** panel at the left, the **Component Services** node is selected by default. Expand **Component Services**, expand **Computers**, and then select **My Computer**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-34.jpg?v=29" alt="Figure 1.33 Screenshot of PLABWIN10: Selecting Component Services &#x26;gt; Computers &#x26;gt; My Computer node in the Component Services window."><figcaption><p>Figure 1.33 Screenshot of PLABWIN10: Selecting Component Services > Computers > My Computer node in the Component Services window.</p></figcaption></figure>

_**Step 4**_

On the **Name** panel in the middle, notice that the COM/DCOM components, apps, and processes are listed that can be managed.

Close the **Component Services** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-35.jpg?v=29" alt="Figure 1.34 Screenshot of PLABWIN10: Displaying the components in the middle pane."><figcaption><p>Figure 1.34 Screenshot of PLABWIN10: Displaying the components in the middle pane.</p></figcaption></figure>

#### **Task 7 - Add a Data Source to a Listed Driver** <a href="#cn-m5-285" id="cn-m5-285"></a>

Configuring ODBC data source is the most convenient way of connecting to a database.

**Note**: You can also connect to a database by using a connection string.

Data source configuration connects a database to one of the available ODBC driver(s), which use Open Database Connectivity (ODBC) interface. With the help of ODBC interface, an application can connect to a database. The added data source is then available for use by any ODBC-enabled application.

You can configure multiple data sources for each installed driver.

In this task, you will add a listed database to one of the listed drivers.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

Double-click **ODBC Data Sources** (64-bit).

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-36.jpg?v=29" alt="Figure 1.35 Screenshot of PLABWIN10: Double-clicking ODBC Data Sources in the Administrative Tools window."><figcaption><p>Figure 1.35 Screenshot of PLABWIN10: Double-clicking ODBC Data Sources in the Administrative Tools window.</p></figcaption></figure>

_**Step 2**_

The **ODBC Data Source Administrator** dialog box is displayed.

Notice that the **User DSN** tab is displayed by default.

Click **Add** to add a data source.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-37.jpg?v=29" alt="Figure 1.36 Screenshot of PLABWIN10: Showing the User DSN tab of the ODBC Data Source Administrator dialog box with the Add button highlighted."><figcaption><p>Figure 1.36 Screenshot of PLABWIN10: Showing the User DSN tab of the ODBC Data Source Administrator dialog box with the Add button highlighted.</p></figcaption></figure>

_**Step 3**_

The **Create New Data Source** dialog box is displayed.

This dialog box lists all the ODBC drivers installed on your system. You can select the one to add.

For this task, select **SQL Server**.

Click **Finish** to save the settings and exit the dialog box.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-38.jpg?v=29" alt="Figure 1.37 Screenshot of PLABWIN10: Showing the Create New Data Source dialog box with the required selection performed and the Finish button highlighted."><figcaption><p>Figure 1.37 Screenshot of PLABWIN10: Showing the Create New Data Source dialog box with the required selection performed and the Finish button highlighted.</p></figcaption></figure>

_**Step 4**_

The **Create a New Data Source to SQL Server** wizard is displayed. In the **Name** textbox, type the following name:

```
SQL
```

Click **Next**.

_**Note:** You need to add the SQL Server name in the Server drop-down. However, the lab environment does not have a SQL Server installed. Therefore, for this task, you can skip it._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-39.jpg?v=29" alt="Figure 1.38 Screenshot of PLABWIN10: Defining a name for the data source in the Name textbox."><figcaption><p>Figure 1.38 Screenshot of PLABWIN10: Defining a name for the data source in the Name textbox.</p></figcaption></figure>

_**Step 5**_

On the next page, deselect **Connect to SQL Server to obtain default settings for the additional configuration options**.

Click **Next**.

_**Note:** Since you do not have a SQL Server installed and keep this option selected, you will be prompted with an error._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-40.jpg?v=29" alt="Figure 1.39 Screenshot of PLABWIN10: Keeping the default option for authentication."><figcaption><p>Figure 1.39 Screenshot of PLABWIN10: Keeping the default option for authentication.</p></figcaption></figure>

_**Step 6**_

On the next page, keep the default settings and click **Next**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-41.jpg?v=29" alt="Figure 1.40 Screenshot of PLABWIN10: Keeping the default option for default database."><figcaption><p>Figure 1.40 Screenshot of PLABWIN10: Keeping the default option for default database.</p></figcaption></figure>

_**Step 7**_

On the next page, keep the default settings and click **Finish**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-42.jpg?v=29" alt="Figure 1.41 Screenshot of PLABWIN10: Clicking Finish to create the data source."><figcaption><p>Figure 1.41 Screenshot of PLABWIN10: Clicking Finish to create the data source.</p></figcaption></figure>

_**Step 8**_

The **ODBC Microsoft SQL Server Setup** dialog box is displayed. Click **OK**.

_**Note:** The intent of this dialog box is to test the data source that you had created. However, in the absence of SQL Server, you will be prompted with an error._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-43.jpg?v=29" alt="Figure 1.42 Screenshot of PLABWIN10: Clicking OK on the ODBC: Microsoft SQL Server Setup dialog box."><figcaption><p>Figure 1.42 Screenshot of PLABWIN10: Clicking OK on the ODBC: Microsoft SQL Server Setup dialog box.</p></figcaption></figure>

_**Step 9**_

Back on the **ODBC Data Source Administrator (64-bit)** dialog box, notice that the newly added data source is now listed on the **User DSN** tab.

_**Note**: A user data source is visible only to the logged in user and can be used only on the current machine._

Click **OK** to save the changes and exit the **ODBC Data Source Administrator** console.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-44.jpg?v=29" alt="Figure 1.43 Screenshot of PLABWIN10: Showing the newly created data source."><figcaption><p>Figure 1.43 Screenshot of PLABWIN10: Showing the newly created data source.</p></figcaption></figure>

#### **Task 8 - Access the Event Viewer Logs** <a href="#cn-m5-353" id="cn-m5-353"></a>

The **Event Viewer** is a system tool in Windows which displays information about various events happening on your computer. This tool can help to track the event flow while troubleshooting any issues either with the OS or the installed applications. The **Event Log** service starts as soon as you start Windows.

There are three types of event logs: application logs, system logs, and security logs. Application and System logs are available to all users; however, security logs are available only to the administrators.

In this task, you will access application logs on the system.

_**Step 1**_

Ensure that the **Administrative Tools** window is displayed.

Double-click **Event Viewer**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-45.jpg?v=29" alt="Figure 1.44 Screenshot of PLABWIN10: Double-clicking Event Viewer in the Administrative Tools window."><figcaption><p>Figure 1.44 Screenshot of PLABWIN10: Double-clicking Event Viewer in the Administrative Tools window.</p></figcaption></figure>

_**Step 2**_

The **Event Viewer** console is displayed.

In the left pane, expand the **Windows Logs** node, and then select the **Application** log.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-46.jpg?v=29" alt="Figure 1.45 Screenshot of PLABWIN10: Showing the Application logs in the middle pane."><figcaption><p>Figure 1.45 Screenshot of PLABWIN10: Showing the Application logs in the middle pane.</p></figcaption></figure>

_**Step 3**_

Notice that various events relevant to the applications on the system are listed in the middle pane. You can have events that are labeled as Information, Warning, and Error.

_**Note:** If the events have not loaded, you may need to maximize the Event Viewer window and click on Windows Logs on the left side of the window and then back onto the Application section._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-47.jpg?v=29" alt="Figure 1.46 Screenshot of PLABWIN10: Showing the Application logs in the middle pane."><figcaption><p>Figure 1.46 Screenshot of PLABWIN10: Showing the Application logs in the middle pane.</p></figcaption></figure>

_**Step 4**_

You can have events that are labeled as Information, Warning, Error and so on. Click **System** in the left pane. Notice that there are different types of events listed.

_**Note:** In your lab environment, there may be a possibility that all of these may not be listed._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-48.jpg?v=29" alt="Figure 1.47 Screenshot of PLABWIN10: Showing the System logs in the middle pane."><figcaption><p>Figure 1.47 Screenshot of PLABWIN10: Showing the System logs in the middle pane.</p></figcaption></figure>

_**Step 5**_

The **Event Viewer** console is displayed. Notice that the Windows Logs node displays different types of logs. It is important to note that these are static logs on all Windows systems. However, a server with specific services, such as a DNS server, can have DNS logs as well. Such logs are listed under the Applications and Services Logs node.

Expand **Applications and Services Logs**. Notice that these logs are specific to applications.

Close all open windows.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m5-c-49.jpg?v=29" alt="Figure 1.48 Screenshot of PLABWIN10: Showing the Applications and Services Logs related logs in the middle pane."><figcaption><p>Figure 1.48 Screenshot of PLABWIN10: Showing the Applications and Services Logs related logs in the middle pane.</p></figcaption></figure>

# Exercise 1 - Using Microsoft Command Line Tools

### **Exercise 1 - Using Microsoft Command Line Tools** <a href="#cn-m4-56" id="cn-m4-56"></a>

Microsoft command line tools are meant to automate certain tasks. These commands are generally used by administrators of the system, not so much by the general user.

These commands automate tasks by using a couple of entities - the scripts and the batch files.

The nature of the tasks performed is not routine, but slightly complex. It is more related to altering the structure of an operating system, rather than merely using it.



#### **Task 1 - Navigation Commands** <a href="#cn-m4-93" id="cn-m4-93"></a>

Navigation commands are used to work around with the directory and sub-directories, with their structural aspects. These commands are used, to get to know the hierarchy of directories and subdirectories, as well as to set path, to the directory or sub-directory, within which work is to be done. In this task, you will learn to use the navigation command, dir.

In this task, you will use the dir command.

_**Step 1**_

Ensure **PLABWIN10** is powered on and connected.

The desktop is displayed.

In the **Type here to search** textbox in the taskbar, type the following command:

```
cmd
```

Under the **Best Match** section, select **Command Prompt**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-2.jpg?v=30" alt="Figure 1.1 Screenshot of device PLABWIN10: Selecting Command Prompt from the Best Match section."><figcaption><p>Figure 1.1 Screenshot of device PLABWIN10: Selecting Command Prompt from the Best Match section.</p></figcaption></figure>

_**Step 2**_

The command prompt window is displayed.

To view the directories and subdirectories inside your current directory, type the following command:

```
dir
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-3.jpg?v=30" alt="Figure 1.2 Screenshot of device PLABWIN10: Showing the output of the dir command."><figcaption><p>Figure 1.2 Screenshot of device PLABWIN10: Showing the output of the dir command.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. If you want to set a particular drive as your current drive, first type the hard disk drive’s name which contains the desired directory. Type the following command:

```
d:
```

Press **Enter**. Notice that the current drive is now **D**:\\>.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-4.jpg?v=30" alt="Figure 1.3 Screenshot of device PLABWIN10: Required command is entered to change to the D drive."><figcaption><p>Figure 1.3 Screenshot of device PLABWIN10: Required command is entered to change to the D drive.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. If you want to set any particular drive as your current drive, first type the hard disk drive’s name, which contains the desired directory. Type the following command:

```
e:
```

Press **Enter**. Notice that the current drive is now **E**:\\>.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-5.jpg?v=30" alt="Figure 1.4 Screenshot of device PLABWIN10: Required command is entered to change to the E drive."><figcaption><p>Figure 1.4 Screenshot of device PLABWIN10: Required command is entered to change to the E drive.</p></figcaption></figure>

_**Step 5**_

You can also set a directory to be the current directory. Type the following command:

```
cd boot/en-us
```

Press **Enter**. This will take you to the **\boot\en-us** subdirectory in the **E** drive.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-6.jpg?v=30" alt="Figure 1.5 Screenshot of device PLABWIN10: Navigating into the boot/en-us folder on the E drive by entering the required command."><figcaption><p>Figure 1.5 Screenshot of device PLABWIN10: Navigating into the boot/en-us folder on the E drive by entering the required command.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. Next, you can view the files and folder of another directory from your current location. You will need to provide the complete path of the directory.

Type the following command:

```
dir c:\users /ah
```

Press **Enter**. The **/a** parameter along with the **/h** attribute displays all hidden files and directories.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-7.jpg?v=30" alt="Figure 1.6 Screenshot of device PLABWIN10: Viewing the files and folder of another directory from your current location."><figcaption><p>Figure 1.6 Screenshot of device PLABWIN10: Viewing the files and folder of another directory from your current location.</p></figcaption></figure>

_**Step 7**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The previous command in **Step 6** shows only the hidden files and folders. If you want to see a specific set of files under a directory, including the subdirectories, type the following command:

```
dir c:\windows\*.exe /s /b
```

Press **Enter**. The **/s** parameter displays all files with the matching criteria in the parent and subdirectories. The **/b** parameter displays only the path and the file names, which makes the output more readable.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-8.jpg?v=30" alt="Figure 1.7 Screenshot of device PLABWIN10: Viewing a specific set of files under a directory, including the subdirectories."><figcaption><p>Figure 1.7 Screenshot of device PLABWIN10: Viewing a specific set of files under a directory, including the subdirectories.</p></figcaption></figure>

_**Step 8**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To navigate back to the original location, which was **c:\users\administrator**, type the following command:

```
c:
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-9.jpg?v=30" alt="Figure 1.8 Screenshot of device PLABWIN10: Navigating back to the original location."><figcaption><p>Figure 1.8 Screenshot of device PLABWIN10: Navigating back to the original location.</p></figcaption></figure>

_**Step 9**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **dir** command uses various parameters. To know more about these parameters, type the following command:

```
dir /?
```

Press **Enter**.

Remember that many of these parameters can be combined with the net use command (covered in **Task 19** of this module).

_**Note:** To see the remaining parameters, press any key._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-10.jpg?v=30" alt="Figure 1.9 Screenshot of device PLABWIN10: Output of the dir command is displayed."><figcaption><p>Figure 1.9 Screenshot of device PLABWIN10: Output of the dir command is displayed.</p></figcaption></figure>

#### **Task 2 - The ipconfig Command** <a href="#cn-m4-168" id="cn-m4-168"></a>

This ipconfig command allows you to view a few network related parameters. Those parameters are - IP address, subnet mask, and default gateway. These parameters are all related to the network, to which your system is connected. Each of them has a specific address, as their value.

In this task, you will learn to use the ipconfig command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To view the IP address(es) assigned to the local system, type the following command:

```
ipconfig
```

Press **Enter.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-11.jpg?v=30" alt="Figure 1.10 Screenshot of device PLABWIN10: Showing the output of the ipconfig command."><figcaption><p>Figure 1.10 Screenshot of device PLABWIN10: Showing the output of the ipconfig command.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To view the complete details of the IP addresses, type the following command:

```
ipconfig /all
```

Press **Enter**. Notice that the output reveals information, such as DNS and DHCP server IP addresses.

_**Note:** A DNS server is required for name resolution. A DHCP server leases IP addresses to the systems on the network._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-12.jpg?v=30" alt="Figure 1.11 Screenshot of device PLABWIN10: Viewing the complete details of the IP addresses on the system."><figcaption><p>Figure 1.11 Screenshot of device PLABWIN10: Viewing the complete details of the IP addresses on the system.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To clear the DNS cache, type the following command:

```
ipconfig /flushdns
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-13.jpg?v=30" alt="Figure 1.12 Screenshot of device PLABWIN10: Clearing the DNS cache."><figcaption><p>Figure 1.12 Screenshot of device PLABWIN10: Clearing the DNS cache.</p></figcaption></figure>

_**Step 4**_

To re-register DNS names, type the following command:

```
ipconfig /registerdns
```

Press **Enter**.

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-14.jpg?v=30" alt="Figure 1.13 Screenshot of device PLABWIN10: Re-registering the DNS names using the specified command."><figcaption><p>Figure 1.13 Screenshot of device PLABWIN10: Re-registering the DNS names using the specified command.</p></figcaption></figure>

_**Step 5**_

To display the DNS Resolver Cache, type the following command:

```
ipconfig /displaydns
```

Press **Enter**.

Press **Enter**. You can scroll up to read the information from the DNS Resolver Cache.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-15.jpg?v=30" alt="Figure 1.14 Screenshot of device PLABWIN10: Displaying the DNS Resolver Cache."><figcaption><p>Figure 1.14 Screenshot of device PLABWIN10: Displaying the DNS Resolver Cache.</p></figcaption></figure>

_**Step 6**_

To release the dynamically assigned IP address(s) on one or more network adapters, type the following command:

```
ipconfig /release
```

Press **Enter**. Notice this command did not have any impact on the assigned IP addresses because these IP addresses are assigned manually.

_**Note**: Even though this device uses static IP addresses, which are assigned manually, its attempt for renewal will take a while._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-16.jpg?v=30" alt="Figure 1.15 Screenshot of device PLABWIN10: Releasing the dynamically assigned IP address(es) on one or more network adapters."><figcaption><p>Figure 1.15 Screenshot of device PLABWIN10: Releasing the dynamically assigned IP address(es) on one or more network adapters.</p></figcaption></figure>

_**Step 7**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. After releasing the IP addresses, you can get the IP addresses from a DHCP server. To do this, type the following command:

```
ipconfig /renew
```

Press **Enter**. Notice this command did not have any impact on the assigned IP addresses because these IP addresses are assigned manually.

Please wait a few minutes for this to process.

In this scenario, you are prompted with an error because there is no DHCP server in the lab environment.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-17.jpg?v=30" alt="Figure 1.16 Screenshot of device PLABWIN10: Renewing the IP addresses on the system."><figcaption><p>Figure 1.16 Screenshot of device PLABWIN10: Renewing the IP addresses on the system.</p></figcaption></figure>

_**Step 8**_

Let’s verify the IP addresses once again on the device. To do this, type the following command:

```
ipconfig
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-18.jpg?v=30" alt="Figure 1.17 Screenshot of device PLABWIN10: Viewing the assigned IP addresses."><figcaption><p>Figure 1.17 Screenshot of device PLABWIN10: Viewing the assigned IP addresses.</p></figcaption></figure>

_**Step 9**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The ipconfig command uses various parameters. To know more about these parameters, type the following command:

```
ipconfig /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-19.jpg?v=30" alt="Figure 1.18 Screenshot of device PLABWIN10: Displaying the help of the ipconfig command."><figcaption><p>Figure 1.18 Screenshot of device PLABWIN10: Displaying the help of the ipconfig command.</p></figcaption></figure>

#### **Task 3 - The ping Command** <a href="#cn-m4-243" id="cn-m4-243"></a>

Ping command is used to check the status of a network device or system on the network. When you execute the ping command, it sends Internet Control Message Protocol (ICMP) Echo Request messages to the destination system.

The source system from which you sent the ICMP messages then waits for a response from the destination system.

In this task, you will use the ping command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To see what parameters are associated with ping command, type the following command:

```
ping
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-20.jpg?v=30" alt="Figure 1.19 Screenshot of device PLABWIN10: Displaying the help of the ping command."><figcaption><p>Figure 1.19 Screenshot of device PLABWIN10: Displaying the help of the ping command.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. Let’s use the **-n** parameter with the ipconfig command. The **-n** parameter sends a pre-defined number of packets to the mentioned IP address, and requests the responses to be returned.

Type the following command:

```
ping -n 3 192.168.0.3
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-21.jpg?v=30" alt="Figure 1.20 Screenshot of device PLABWIN10: Entering the specified command to send packets to the mentioned IP address."><figcaption><p>Figure 1.20 Screenshot of device PLABWIN10: Entering the specified command to send packets to the mentioned IP address.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can also find the hostname of a system with the **-a** parameter. Type the following command:

```
ping -a 192.168.0.3
```

Press **Enter**. Notice that the name is returned as **PLABWIN810**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-22.jpg?v=30" alt="Figure 1.21 Screenshot of device PLABWIN10: Finding the hostname of a system with the -a parameter."><figcaption><p>Figure 1.21 Screenshot of device PLABWIN10: Finding the hostname of a system with the -a parameter.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. Let’s ping to the same device with its name. Type the following command:

```
ping plabwin810
```

Press **Enter**. Notice that the ping is successful.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-23.jpg?v=30" alt="Figure 1.22 Screenshot of device PLABWIN10: Pinging a network device with its name."><figcaption><p>Figure 1.22 Screenshot of device PLABWIN10: Pinging a network device with its name.</p></figcaption></figure>

_**Step 5**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can run the ping command indefinitely. Type the following command:

```
ping -t 192.168.0.3
```

Press **Enter**.

Notice that the ping is running indefinitely.

Press **Ctrl+c** to break the command.

_**Note:** If you are unable to break the command, close the Command Prompt window with the X in the top right. Afterward, search the system for Command Prompt to then open it again and continue to the next step._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-24.jpg?v=30" alt="Figure 1.23 Screenshot of device PLABWIN10: Running the ping command indefinitely."><figcaption><p>Figure 1.23 Screenshot of device PLABWIN10: Running the ping command indefinitely.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. Ensure that the **PLABCENTOS** device is up and running. Let’s now try to ping a Linux system.

Type the following command:

```
ping plabcentos
```

Press **Enter**. Notice that the ping returns an error.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-25.jpg?v=30" alt="Figure 1.24 Screenshot of device PLABWIN10: Pinging the PLABCENTOS device."><figcaption><p>Figure 1.24 Screenshot of device PLABWIN10: Pinging the PLABCENTOS device.</p></figcaption></figure>

_**Step 7**_

Let’s now attempt to ping the IP address of **PLABCENTOS**. Type the following command:

```
ping 192.168.0.5
```

Press **Enter**. Notice that there is no error.

_**Note:** There are two methods you can use to get a response from the Linux device name: either through DHCP or adding the device name in the source system’s /etc/hosts file. After using either method, you will be able to ping PLABCENTOS with its name._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-26.jpg?v=30" alt="Figure 1.25 Screenshot of device PLABWIN10: Pinging the IP address of the PLABCENTOS device."><figcaption><p>Figure 1.25 Screenshot of device PLABWIN10: Pinging the IP address of the PLABCENTOS device.</p></figcaption></figure>

#### **Task 4 - The tracert Command** <a href="#cn-m4-308" id="cn-m4-308"></a>

The tracert command is used to trace the path of an IP (Internet Protocol) packet. A packet has a destination address, along with initial count, which is set to 1. Each device along the network path increases the count by one. The network devices are called nodes. When the result is shown, it contains the hop count, as well as the node information.

In this task, you will learn to use the tracert command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To trace the path to a destination system, type the following command:

```
tracert 192.168.0.1
```

Press **Enter**. Notice that the IP address is resolved to the device name.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-27.jpg?v=30" alt="Figure 1.26 Screenshot of device PLABWIN10: Tracing the path to a networked system."><figcaption><p>Figure 1.26 Screenshot of device PLABWIN10: Tracing the path to a networked system.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To trace the path to a device without performing name resolution, type the following command:

```
tracert -d 192.168.0.1
```

Press **Enter**. Notice that the response is much quicker.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-28.jpg?v=30" alt="Figure 1.27 Screenshot of device PLABWIN10: Tracing the path to a device without performing name resolution."><figcaption><p>Figure 1.27 Screenshot of device PLABWIN10: Tracing the path to a device without performing name resolution.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can perform path tracing to a domain name or a specific server on the Internet. Type the following command:

```
tracert -d 8.8.8.8
```

Press **Enter**.

_**Note:** Some environments have firewall configurations that intentionally do not respond to ICMP packets (the protocol used by tracert), this can be due to security configurations. In this circumstance the hop out is most likely to be **“\* \* \* \* Request timed out**”. Please run this command on your PC to see an alternative result._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-29.jpg?v=30" alt="Figure 1.28 Screenshot of device PLABWIN10: Performing the path tracing to a domain name or a specific server on the Internet."><figcaption><p>Figure 1.28 Screenshot of device PLABWIN10: Performing the path tracing to a domain name or a specific server on the Internet.</p></figcaption></figure>

_**Step 4**_

Let’s trace the path to the **http://intranet** Website. Type the following command:

```
tracert intranet
```

Press **Enter**. Notice that the first hop did not provide the information in a timely manner. Then, the second hop was Intranet.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-30.jpg?v=30" alt="Figure 1.29 Screenshot of device PLABWIN10: Tracing the path to the http://intranet Website."><figcaption><p>Figure 1.29 Screenshot of device PLABWIN10: Tracing the path to the http://intranet Website.</p></figcaption></figure>

_**Step 5**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. Let’s trace the path to the **http://intranet** website but with a defined timeout. Type the following command:

```
tracert -w 500 intranet
```

Press **Enter**. Notice that the first hop did respond within the defined timeout. If you still get the timeout error, this is an expected result as your Tracert is hitting our firewall which is causing the first timeout.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-31.jpg?v=30" alt="Figure 1.30 Screenshot of device PLABWIN10: Tracing the path to the http://intranet Website but with a defined timeout."><figcaption><p>Figure 1.30 Screenshot of device PLABWIN10: Tracing the path to the http://intranet Website but with a defined timeout.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **tracert** command uses various parameters. To know more about these parameters, type the following command:

```
tracert
```

Press **Enter**. Remember that many of these parameters can be combined with the net use command (covered in **Task 19** of this module).

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-32.jpg?v=30" alt="Figure 1.31 Screenshot of device PLABWIN10: Displaying the help of the tracert command."><figcaption><p>Figure 1.31 Screenshot of device PLABWIN10: Displaying the help of the tracert command.</p></figcaption></figure>

#### **Task 5 - The netstat Command** <a href="#cn-m4-360" id="cn-m4-360"></a>

As the name suggests, the netstat command provides network-related statistics. Various parameters can be used along with this command.

In this task, you will learn to use the netstat command. Step 1

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To view the output of the **netstat** command without any parameter, type the following command:

```
netstat
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-33.jpg?v=30" alt="Figure 1.32 Screenshot of device PLABWIN10: Displaying the output of the netstat command without any parameter."><figcaption><p>Figure 1.32 Screenshot of device PLABWIN10: Displaying the output of the netstat command without any parameter.</p></figcaption></figure>

The netstat command shows all the active Transmission Control Protocol (TCP) connections and their state.

_**Note:** The Transmission Control Protocol (TCP) connection is a reliable, ordered delivery of a stream of bytes, which are sent from one system to another system on the network. It is the core protocol being used in World Wide Web and applications, such as E-mail. The User Datagram Protocol (UDP) does not provide reliable data service but utilizes reduced latency._

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To view the state of all TCP connections with each connection's Process ID (PID), type the following command:

```
netstat -o
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-34.jpg?v=30" alt="Figure 1.34 Screenshot of device PLABWIN10: Viewing the state of the TCP connections."><figcaption><p>Figure 1.34 Screenshot of device PLABWIN10: Viewing the state of the TCP connections.</p></figcaption></figure>

_**Step 3**_

To view the information about a particular protocol, such as TCP, type the following command:

```
netstat -s -p tcp
```

Press **Enter**. You may need to wait a few minutes for this to process.

_**Note**: The output will vary in this lab environment. The active connections present will differ at the time this command is executed._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-35.jpg?v=30" alt="Figure 1.35 Screenshot of device PLABWIN10: Viewing the information about a particular protocol."><figcaption><p>Figure 1.35 Screenshot of device PLABWIN10: Viewing the information about a particular protocol.</p></figcaption></figure>

_**Step 4**_

To update the connection statistics every few seconds, such as **5** seconds, type the following command:

```
netstat -e -t 5
```

Press **Enter**. The command will continue to generate the output.

Press **Ctrl+c** to break the command.

_**Note:** If you are unable to break the command, close the Command Prompt window with the X in the top right. Afterward, search the system for Command Prompt to then open it again and continue to the next step._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-36.jpg?v=30" alt="Figure 1.36 Screenshot of device PLABWIN10: Updating the connection statistics every 5 seconds."><figcaption><p>Figure 1.36 Screenshot of device PLABWIN10: Updating the connection statistics every 5 seconds.</p></figcaption></figure>

_**Step 5**_

To list all TCP and UDP connections, type the following command:

```
netstat -a
```

Press **Enter**. Notice that there are TCP and UDP connections.

_**Note:** The Transmission Control Protocol (TCP) connection is a reliable, ordered delivery of a stream of bytes, which are sent from one system to another system on the network. It is the core protocol being used in World Wide Web and applications, such as E-mail. The User Datagram Protocol (UDP) does not provide reliable data service but utilizes reduced latency._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-37.jpg?v=30" alt="Figure 1.37 Screenshot of device PLABWIN10: Listing all TCP and UDP connections."><figcaption><p>Figure 1.37 Screenshot of device PLABWIN10: Listing all TCP and UDP connections.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **netstat** command uses various parameters. To know more about these parameters, type the following command:

```
netstat /?
```

Press **Enter**. Remember that many of these parameters can be combined with the net use command.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-38.jpg?v=30" alt="Figure 1.38 Screenshot of device PLABWIN10: Displaying the help of the netstat command."><figcaption><p>Figure 1.38 Screenshot of device PLABWIN10: Displaying the help of the netstat command.</p></figcaption></figure>

#### **Task 6 - The nslookup Command** <a href="#cn-m4-413" id="cn-m4-413"></a>

The nslookup command displays information which is useful for identifying issues related to this domain name system (DNS). This command can be used with different parameters. Each version of command displays a specific set of information, which highlights a specific aspect of a domain name system.

In this task, you will learn to use the nslookup command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can use the nslookup command without any parameters. Type the following command:

```
nslookup
```

Press **Enter**. Notice that the command expects inputs from the user.

For the time being, press **Ctrl+c** keys to break the command.

_**Note:** If you are unable to break the command, close the Command Prompt window with the X in the top right. Afterward, search the system for Command Prompt to then open it again and continue to the next step._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-39.jpg?v=30" alt="Figure 1.39 Screenshot of device PLABWIN10: Using the nslookup command without any parameters."><figcaption><p>Figure 1.39 Screenshot of device PLABWIN10: Using the nslookup command without any parameters.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To find the **A** record for a domain, type the following command:

```
nslookup practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-40.jpg?v=30" alt="Figure 1.40 Screenshot of device PLABWIN10: Finding the A record for a domain with the nslookup command."><figcaption><p>Figure 1.40 Screenshot of device PLABWIN10: Finding the A record for a domain with the nslookup command.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To find the NS (name server) record for a domain, type the following command:

```
nslookup -type=ns practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-41.jpg?v=30" alt="Figure 1.41 Screenshot of device PLABWIN10: Finding the NS record for a domain with the nslookup command."><figcaption><p>Figure 1.41 Screenshot of device PLABWIN10: Finding the NS record for a domain with the nslookup command.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To query the SOA (Start of Authority) record for a domain, type the following command:

```
nslookup -type=soa practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-42.jpg?v=30" alt="Figure 1.42 Screenshot of device PLABWIN10: Querying the SOA record for a domain with the nslookup command."><figcaption><p>Figure 1.42 Screenshot of device PLABWIN10: Querying the SOA record for a domain with the nslookup command.</p></figcaption></figure>

_**Step 5**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To find all DNS records for a domain, type the following command:

```
nslookup -type=any practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-43.jpg?v=30" alt="Figure 1.43 Screenshot of device PLABWIN10: Finding all DNS records for a domain with the nslookup command."><figcaption><p>Figure 1.43 Screenshot of device PLABWIN10: Finding all DNS records for a domain with the nslookup command.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To use a specific DNS server for a domain, type the following command:

```
nslookup practicelabs.com plabdc01.practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-44.jpg?v=30" alt="Figure 1.44 Screenshot of device PLABWIN10: Using a specific DNS server for a domain with the nslookup command."><figcaption><p>Figure 1.44 Screenshot of device PLABWIN10: Using a specific DNS server for a domain with the nslookup command.</p></figcaption></figure>

_**Step 7**_

To perform a reverse lookup from an IP address, type the following command:

```
nslookup 192.168.0.1
```

Press **Enter**. Notice there is a timeout.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-45.jpg?v=30" alt="Figure 1.45 Screenshot of device PLABWIN10: Performing a reverse lookup from an IP address with the nslookup command."><figcaption><p>Figure 1.45 Screenshot of device PLABWIN10: Performing a reverse lookup from an IP address with the nslookup command.</p></figcaption></figure>

_**Step 8**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To increase the timeout, type the following command:

```
nslookup -timeout=200 practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-46.jpg?v=30" alt="Figure 1.46 Screenshot of device PLABWIN10: Increasing the timeout limit of the nslookup command."><figcaption><p>Figure 1.46 Screenshot of device PLABWIN10: Increasing the timeout limit of the nslookup command.</p></figcaption></figure>

_**Step 9**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can also use the **-debug** parameter with the nslookup command. It generates the questions and answers with the detailed information. Type the following command:

```
nslookup -debug practicelabs.com
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-47.jpg?v=30" alt="Figure 1.47 Screenshot of device PLABWIN10: Using the -debug parameter along with the nslookup command."><figcaption><p>Figure 1.47 Screenshot of device PLABWIN10: Using the -debug parameter along with the nslookup command.</p></figcaption></figure>

_**Step 10**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **nslookup** command uses various parameters. To know more about these parameters, type the following command:

```
nslookup /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-48.jpg?v=30" alt="Figure 1.48 Screenshot of device PLABWIN10: Displaying the help of the nslookup command."><figcaption><p>Figure 1.48 Screenshot of device PLABWIN10: Displaying the help of the nslookup command.</p></figcaption></figure>

#### **Task 7 - The shutdown Command** <a href="#cn-m4-497" id="cn-m4-497"></a>

The shutdown command is used to shut down the machine or restart it. It can be used for the local system, as well as for a remote system, connected over the network.

The limitation of the ‘shutdown’ command is that it can be used on one machine at a time. If you want to use the command on multiple machines, then you have to type the command the number of times as your machine count.

In this task, you will learn to use the shutdown command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To restart the system, type the following command:

```
shutdown /r
```

Press **Enter**.

_**Step 2**_

You are prompted with a message for signing out.

Click **Close**.

![Practice Labs screenshot.](https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-49.jpg?v=30)

_Figure 1.49 Screenshot of device PLABWIN10: Displaying the signing out the message._

_**Step 3**_

The **PLABWIN10** device now reboots. You need to go to the Practice Labs environment and invoke **PLABWIN10** once again.

Open the command prompt (as shown in **Task 1, Step 1**).

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-50.jpg?v=30" alt="Figure 1.50 Screenshot of device PLABWIN10: Opening the command prompt."><figcaption><p>Figure 1.50 Screenshot of device PLABWIN10: Opening the command prompt.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To restart the system immediately, type the following command:

```
shutdown /r /t 0
```

Press **Enter**.

Notice this time you did not get a message dialog box. This is because you had defined the restart with the value of 0, which means immediately without a wait.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-51.jpg?v=30" alt="Figure 1.51 Screenshot of device PLABWIN10: Restarting the system immediately."><figcaption><p>Figure 1.51 Screenshot of device PLABWIN10: Restarting the system immediately.</p></figcaption></figure>

_**Step 5**_

The **shutdown** command uses various parameters. To know more about these parameters, type the following command:

```
shutdown /?
```

Press **Enter**. You would need to scroll up and go through various parameters.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-52.jpg?v=30" alt="Figure 1.52 Screenshot of device PLABWIN10: Displaying the help of the shutdown command."><figcaption><p>Figure 1.52 Screenshot of device PLABWIN10: Displaying the help of the shutdown command.</p></figcaption></figure>

#### **Task 8 - The dism Command** <a href="#cn-m4-533" id="cn-m4-533"></a>

The dism stands for deployment image servicing and management. This utility is used to identify the issues with your windows system files and fix the errors. For example, if a few issues are observed while booting up your machine, this command can be used to detect the errors.

This command has three key parameters. One is checking health; another is scan health and third is restore health.

In this task, you will learn to use the dism command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The dism command with the **/checkhealth** parameter detects the corruption but does not repair it. Type the following command:

```
dism /online /cleanup-image /checkhealth
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-53.jpg?v=30" alt="Figure 1.53 Screenshot of device PLABWIN10: Displaying the output of the /checkhealth parameter of the dism command."><figcaption><p>Figure 1.53 Screenshot of device PLABWIN10: Displaying the output of the /checkhealth parameter of the dism command.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **dism** command with the **/ScanHealth** parameter scans for issues in the Windows image. Type the following command:

```
dism /online /cleanup-image /scanhealth
```

Press **Enter**. This command may take a few minutes to complete.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-54.jpg?v=30" alt="Figure 1.54 Screenshot of device PLABWIN10: Displaying the execution of the /scanhealth parameter of the dism command."><figcaption><p>Figure 1.54 Screenshot of device PLABWIN10: Displaying the execution of the /scanhealth parameter of the dism command.</p></figcaption></figure>

_**Step 3**_

After running the scan, the command output is displayed.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-55.jpg?v=30" alt="Figure 1.55 Screenshot of device PLABWIN10: Displaying the output of the /scanhealth parameter of the dism command."><figcaption><p>Figure 1.55 Screenshot of device PLABWIN10: Displaying the output of the /scanhealth parameter of the dism command.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **dism** command with the **/restorehealth** parameter scans for issues in the Windows image and then repairs the issues automatically.

Type the following command:

```
dism /online /cleanup-image /restorehealth
```

Press **Enter**. This command will take a few minutes to complete.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-56.jpg?v=30" alt="Figure 1.56 Screenshot of device PLABWIN10: Displaying the execution of the /restorehealth parameter of the dism command."><figcaption><p>Figure 1.56 Screenshot of device PLABWIN10: Displaying the execution of the /restorehealth parameter of the dism command.</p></figcaption></figure>

_**Step 5**_

After running the scan, the command output is displayed.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-57.jpg?v=30" alt="Figure 1.57 Screenshot of device PLABWIN10: Displaying the output of the /restorehealth parameter of the dism command."><figcaption><p>Figure 1.57 Screenshot of device PLABWIN10: Displaying the output of the /restorehealth parameter of the dism command.</p></figcaption></figure>

_**Step 6**_

The **dism** command uses various parameters. To know more about these parameters, type the following command:

```
dism /?
```

Press **Enter**. You would need to scroll up and go through various parameters.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-58.jpg?v=30" alt="Figure 1.58 Screenshot of device PLABWIN10: Displaying the help of the dism command."><figcaption><p>Figure 1.58 Screenshot of device PLABWIN10: Displaying the help of the dism command.</p></figcaption></figure>

_**Step 7**_

Close the command prompt by typing the following command:

```
exit
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-59.jpg?v=30" alt="Figure 1.59 Screenshot of device PLABWIN10: Exiting the command prompt window."><figcaption><p>Figure 1.59 Screenshot of device PLABWIN10: Exiting the command prompt window.</p></figcaption></figure>

#### **Task 9 - The sfc Command** <a href="#cn-m4-583" id="cn-m4-583"></a>

SFC is short for System File Checker. As the name indicates, it performs fault identification and corrections of system files. If some system functions are not working, or the operating system is crashing, you can use sfc to detect issues and perform corrective measures.

In this task, you will learn to use the sfc command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

In the **Type here to search** textbox in the taskbar, type the following command:

```
cmd
```

Under **Best Match** section, right-click **Command Prompt** and select **Run as administrator**.

![Practice Labs screenshot.](https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-60.jpg?v=30)_Figure 1.60 Screenshot of device PLABWIN10: Opening the command prompt with the administrative privileges._

_**Step 2**_

The **/scannow** parameter of the **sfc** command checks the protected system files and repairs them if required. Type the following command:

```
sfc /scannow
```

Press **Enter**. Notice that there were integrity issues encountered, which have been repaired successfully.

_**Note**: This command may take longer than **10-20 minutes** to complete, if you would like to skip this step please press **ctrl + c** and move to the next step._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-61.jpg?v=30" alt="Figure 1.61 Screenshot of device PLABWIN10: Displaying the result of the sfc command."><figcaption><p>Figure 1.61 Screenshot of device PLABWIN10: Displaying the result of the sfc command.</p></figcaption></figure>

_**Step 3**_

You can use the sfc command to repair a specific file. Type the following command:

```
sfc /scanfile=c:\windows\system32\ieframe.dll
```

Press **Enter**. Notice that no integrity violations are reported.

_**Note**: This process may take a few minutes._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-62.jpg?v=30" alt="Figure 1.62 Screenshot of device PLABWIN10: Repairing a file with the sfc command."><figcaption><p>Figure 1.62 Screenshot of device PLABWIN10: Repairing a file with the sfc command.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can use the verify the protected files with the **/verifyonly** parameter of the sfc command. Type the following command:

```
sfc /verifyonly
```

Press **Enter**.

_**Note**: Notice the message **This process may take some time** in the command prompt window._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-63.jpg?v=30" alt="Figure 1.63 Screenshot of device PLABWIN10: Verifying the protected files with the /verifyonly parameter of the sfc command."><figcaption><p>Figure 1.63 Screenshot of device PLABWIN10: Verifying the protected files with the /verifyonly parameter of the sfc command.</p></figcaption></figure>

_**Step 5**_

This process runs for quite a long time. It may take **more than an hour** to complete. For this task, you can break the command by pressing **Ctrl+c**.

_**Note:** If you are unable to break the command, close the Command Prompt window with the X in the top right. Afterward, search the system for Command Prompt to then open it again and continue to the next step._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-64.jpg?v=30" alt="Figure 1.64 Screenshot of device PLABWIN10: Showing the execution of the /verifyonly parameter along with the sfc command."><figcaption><p>Figure 1.64 Screenshot of device PLABWIN10: Showing the execution of the /verifyonly parameter along with the sfc command.</p></figcaption></figure>

_**Step 6**_

The **sfc** command uses various parameters. To know more about these parameters, type the following command:

```
sfc /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-65.jpg?v=30" alt="Figure 1.65 Screenshot of device PLABWIN10: Displaying the help of the sfc command."><figcaption><p>Figure 1.65 Screenshot of device PLABWIN10: Displaying the help of the sfc command.</p></figcaption></figure>

#### **Task 10 - The chkdsk Command** <a href="#cn-m4-627" id="cn-m4-627"></a>

The ckhdsk command scans the specified sector of a local hard disk drive or the specified external storage device, attached to the computer system.

For example, it could be a USB flash drive, or a disk, in a CD/DVD drive. This command will mark the damaged/erroneous sector(s) as bad and will recover the information contained by that sector(s), if still readable.

The command has various parameters, which can be used along with it, which perform various different tasks.

In this task, you will learn to use the chkdsk command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can run the **chkdsk** command in read-only mode. Type the following command:

```
chkdsk
```

Press **Enter**.

_**Note:** You can maximize the command prompt window if required._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-66.jpg?v=30" alt="Figure 1.66 Screenshot of device PLABWIN10: Displaying the output of the chkdsk command."><figcaption><p>Figure 1.66 Screenshot of device PLABWIN10: Displaying the output of the chkdsk command.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You will now skip checking cycles in the folder structure with the help of **/C** parameter. Type the following command:

```
chkdsk /C
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-67.jpg?v=30" alt="Figure 1.67 Screenshot of device PLABWIN10: Skipping checking cycles in the folder structure with the help of /C parameter."><figcaption><p>Figure 1.67 Screenshot of device PLABWIN10: Skipping checking cycles in the folder structure with the help of /C parameter.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can also use the **/f** parameter to fix the hard drive errors. Along with this, you can also use the /r parameter to locate bad sectors. Type the following command:

```
chkdsk c: /f /r
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-68.jpg?v=30" alt="Figure 1.68 Screenshot of device PLABWIN10: Using the /f parameter with the chkdsk command."><figcaption><p>Figure 1.68 Screenshot of device PLABWIN10: Using the /f parameter with the chkdsk command.</p></figcaption></figure>

_**Step 4**_

When prompted for confirmation, type the following:

```
Y
```

Press **Enter**. Notice that the C drive will be checked on the next system restart.

_**Note:** If time permits, you can restart the system right now and see the check being performed._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-69.jpg?v=30" alt="Figure 1.69 Screenshot of device PLABWIN10: Confirming the execution of the chkdsk command with the /f parameter."><figcaption><p>Figure 1.69 Screenshot of device PLABWIN10: Confirming the execution of the chkdsk command with the /f parameter.</p></figcaption></figure>

_**Step 5**_

The **chkdsk** command uses various parameters. To know more about these parameters, type the following command:

```
chkdsk /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-70.jpg?v=30" alt="Figure 1.70 Screenshot of device PLABWIN10: Displaying the help of the chkdsk command."><figcaption><p>Figure 1.70 Screenshot of device PLABWIN10: Displaying the help of the chkdsk command.</p></figcaption></figure>

#### **Task 11 - The diskpart Command** <a href="#cn-m4-671" id="cn-m4-671"></a>

The diskpart command is used to perform partitioning activity. If you want to create a new primary segment inside one of your existing drives, or if you want to delete a particular drive of your storage device, it all can be done using the diskpart command.

In short, the diskpart command allows you to create, delete, and resize the partitions of your hard disk drive(s), as well as your external storage device’s drive(s).

In this task, you will learn to use the diskpart command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The set of commands mentioned below will get you to a specific disk of the machine’s hard drive. Once you reach there, a number of different activities, such as creating a primary partition, can be performed.

To start diskpart, type the following command:

```
diskpart
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-71.jpg?v=30" alt="Figure 1.71 Screenshot of device PLABWIN10: Starting the diskpart shell."><figcaption><p>Figure 1.71 Screenshot of device PLABWIN10: Starting the diskpart shell.</p></figcaption></figure>

_**Step 2**_

To list the available disks in the system, type the following command:

```
list disk
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-72.jpg?v=30" alt="Figure 1.72 Screenshot of device PLABWIN10: Listing the available disks in the system."><figcaption><p>Figure 1.72 Screenshot of device PLABWIN10: Listing the available disks in the system.</p></figcaption></figure>

_**Step 3**_

To select a disk, type the following command:

```
select disk 1
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-73.jpg?v=30" alt="Figure 1.73 Screenshot of device PLABWIN10: Selecting a disk from the available disks."><figcaption><p>Figure 1.73 Screenshot of device PLABWIN10: Selecting a disk from the available disks.</p></figcaption></figure>

_**Step 4**_

To list the available disks in the system, type the following command:

```
list disk
```

Press **Enter**. Notice that the selected disk has an \* (asterisk) before it.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-74.jpg?v=30" alt="Figure 1.74 Screenshot of device PLABWIN10: Listing the disks and showing the selected disk."><figcaption><p>Figure 1.74 Screenshot of device PLABWIN10: Listing the disks and showing the selected disk.</p></figcaption></figure>

_**Step 5**_

To list the partitions on the selected disk, type the following command:

```
list partition
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-75.jpg?v=30" alt="Figure 1.75 Screenshot of device PLABWIN10: Listing the partitions on the selected disks."><figcaption><p>Figure 1.75 Screenshot of device PLABWIN10: Listing the partitions on the selected disks.</p></figcaption></figure>

_**Step 6**_

To select a partition, type the following command:

```
select partition 2
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-76.jpg?v=30" alt="Figure 1.76 Screenshot of device PLABWIN10: Selecting a partition."><figcaption><p>Figure 1.76 Screenshot of device PLABWIN10: Selecting a partition.</p></figcaption></figure>

_**Step 7**_

To make the partition active, type the following command:

```
active
```

Press **Enter**.

Notice that a message is flashed that the partition cannot be marked as active because it is not a fixed MBR disk.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-77.jpg?v=30" alt="Figure 1.77 Screenshot of device PLABWIN10: Attempting to make a partition active."><figcaption><p>Figure 1.77 Screenshot of device PLABWIN10: Attempting to make a partition active.</p></figcaption></figure>

_**Step 8**_

You will need to quick format the partition with the NTFS file system, and then assign drive letter **F** to it.

Type the following command:

```
Format FS=NTFS label=F quick
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-78.jpg?v=30" alt="Figure 1.78 Screenshot of device PLABWIN10: Performing a quick format of the selected partition."><figcaption><p>Figure 1.78 Screenshot of device PLABWIN10: Performing a quick format of the selected partition.</p></figcaption></figure>

_**Step 9**_

To exit from diskpart, type the following command:

```
exit
```

Press **Enter**. You are back on the command prompt.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-79.jpg?v=30" alt="Figure 1.79 Screenshot of device PLABWIN10: Exiting from the diskpart shell."><figcaption><p>Figure 1.79 Screenshot of device PLABWIN10: Exiting from the diskpart shell.</p></figcaption></figure>

_**Note:** You can get the list of commands by invoking diskpart and then typing help._

#### **Task 12 - The taskkill Command** <a href="#cn-m4-736" id="cn-m4-736"></a>

The taskkill command allows you to end a particular task or a process under execution. It is done by mentioning one of the parameters of that particular task.

You either need to specify the image, name or the PID associated with the task you wish to end.

In this task, you will learn to use the taskkill command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To list the tasks or processes, type the following command:

```
tasklist
```

Press **Enter**. Notice that the tasks or processes are displayed. Each task or process has a process ID assigned.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-80.jpg?v=30" alt="Figure 1.80 Screenshot of device PLABWIN10: Listing the tasks or processes."><figcaption><p>Figure 1.80 Screenshot of device PLABWIN10: Listing the tasks or processes.</p></figcaption></figure>

_**Step 2**_

In the **Type here to search** textbox in the taskbar, type the following command:

```
notepad
```

Under **Best Match** section, select **Notepad**. Minimize Notepad after it is opened.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-81.jpg?v=30" alt="Figure 1.81 Screenshot of device PLABWIN10: Opening Notepad from the Best Match section."><figcaption><p>Figure 1.81 Screenshot of device PLABWIN10: Opening Notepad from the Best Match section.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To forcefully kill the open Notepad window, type the following command:

```
taskkill /f /im notepad.exe
```

Press **Enter**. Notice that the notepad.exe process is now terminated. The Notepad window has also terminated.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-82.jpg?v=30" alt="Figure 1.82 Screenshot of device PLABWIN10: Killing the open Notepad window forcefully."><figcaption><p>Figure 1.82 Screenshot of device PLABWIN10: Killing the open Notepad window forcefully.</p></figcaption></figure>

_**Step 4**_

To list the tasks or processes, type the following command:

```
tasklist
```

Press **Enter**. Notice that the tasks or processes are displayed. Each task or process has a process ID assigned.

Take a note of a **PID** from the second column of the task list result set. You will need this ID for the following step. Is this current lab environment, the PID was 6740.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-83.jpg?v=30" alt="Figure 1.83 Screenshot of device PLABWIN10: Listing the tasks or processes."><figcaption><p>Figure 1.83 Screenshot of device PLABWIN10: Listing the tasks or processes.</p></figcaption></figure>

_**Step 5**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To kill a process using its PID, type the following command:

```
taskkill /pid
```

Press the **space bar** then type in the **PID** you noted from step 4.

Press **Enter**. Notice that the process is being terminated.

_**Note**: The PID changes every time._\
_In the lab environment example, the command looks like this **taskkill /pid 6740**. Ensure you select one from the result set of tasklist command executed earlier._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-84.jpg?v=30" alt="Figure 1.84 Screenshot of device PLABWIN10: Killing a process using its PID."><figcaption><p>Figure 1.84 Screenshot of device PLABWIN10: Killing a process using its PID.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **taskkill** command uses various parameters. To know more about these parameters, type the following command:

```
taskkill /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-85.jpg?v=30" alt="Figure 1.85 Screenshot of device PLABWIN10: Displaying the help of the taskkill command."><figcaption><p>Figure 1.85 Screenshot of device PLABWIN10: Displaying the help of the taskkill command.</p></figcaption></figure>

#### **Task 13 - The gpupdate Command** <a href="#cn-m4-788" id="cn-m4-788"></a>

An individual user or a machine has a certain set of domain and local policies applied to it. A policy could be local or domain-based. When a domain-based policy is created, it takes a while before the policy is applied to the systems on the network.

A user can run the gpupdate (group policy update) command on the local system to apply the policy. The domain in which a policy is created, the recipient system must be part of it.

In this task, you will learn to use the gpupdate command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To run the gpupdate command without any parameter, type the following command:

```
gpupdate
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-86.jpg?v=30" alt="Figure 1.86 Screenshot of device PLABWIN10: Showing the output of the gpupdate command."><figcaption><p>Figure 1.86 Screenshot of device PLABWIN10: Showing the output of the gpupdate command.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To apply all the policies, not only the ones that have changed, type the following command:

```
gpupdate /force
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-87.jpg?v=30" alt="Figure 1.87 Screenshot of device PLABWIN10: Applying all the policies, not only the ones that have changed."><figcaption><p>Figure 1.87 Screenshot of device PLABWIN10: Applying all the policies, not only the ones that have changed.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. When you run the gpupdate command, by default, user and computer policies are applied. You can choose to apply either user or computer.

Type the following command:

```
gpupdate /Target:User
```

Press **Enter**.

_**Note:** If you provide a blank space after the colon, then the command will not run. Instead, it will show the help for gpupdate._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-88.jpg?v=30" alt="Figure 1.88 Screenshot of device PLABWIN10: Updating a specific set of policies."><figcaption><p>Figure 1.88 Screenshot of device PLABWIN10: Updating a specific set of policies.</p></figcaption></figure>

_**Step 4**_

The default number of seconds to wait for policy processing is **600** seconds. You can remove the wait time. Type the following command:

```
gpupdate /Wait:0
```

Press **Enter**.

_**Note:** If you provide a blank space after the colon, then the command will not run. Instead, it will show the help for gpupdate._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-89.jpg?v=30" alt="Figure 1.89 Screenshot of device PLABWIN10: Removing the wait time for the policy update."><figcaption><p>Figure 1.89 Screenshot of device PLABWIN10: Removing the wait time for the policy update.</p></figcaption></figure>

_**Step 5**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **gpupdate** command uses various parameters. To know more about these parameters, type the following command:

```
gpupdate /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-90.jpg?v=30" alt="Figure 1.90 Screenshot of device PLABWIN10: Displaying the help of the gpupdate command."><figcaption><p>Figure 1.90 Screenshot of device PLABWIN10: Displaying the help of the gpupdate command.</p></figcaption></figure>

#### **Task 14 - The gpresult Command** <a href="#cn-m4-834" id="cn-m4-834"></a>

For each user or the machine, there is a set of policies which gets applied. These policies are about how to the application programs, resources based on the network and the operating system behave for that particular user or a computer.

These policies can overlap in nature. The gpresult command generates the resultant set of the applicable policies after considering the overlapping.

In this task, you will learn to use the gpresult command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To display the RSoP summary data, type the following command:

```
gpresult /r
```

Press **Enter**.

_**Note:** Maximize the command prompt window if required._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-91.jpg?v=30" alt="Figure 1.91 Screenshot of device PLABWIN10: Displaying the RSoP summary data."><figcaption><p>Figure 1.91 Screenshot of device PLABWIN10: Displaying the RSoP summary data.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To display all the information about Group Policy, type the following command:

```
gpresult /z
```

Press **Enter**.

_**Note:** The output of this command spans through multiple pages. You will need to scroll and read the information. The screenshot below displays the information from the start of the output of the command._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-92.jpg?v=30" alt="Figure 1.92 Screenshot of device PLABWIN10: Displaying all the information about Group Policy."><figcaption><p>Figure 1.92 Screenshot of device PLABWIN10: Displaying all the information about Group Policy.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To display policy details of a remote computer, type the following command:

```
gpresult /s plabdc01 /r
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-93.jpg?v=30" alt="Figure 1.93 Screenshot of device PLABWIN10: Displaying the policy details of a remote computer."><figcaption><p>Figure 1.93 Screenshot of device PLABWIN10: Displaying the policy details of a remote computer.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **gpresult** command uses various parameters. To know more about these parameters, type the following command:

```
gpresult /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-94.jpg?v=30" alt="Figure 1.94 Screenshot of device PLABWIN10: Displaying the help of the gpresult command."><figcaption><p>Figure 1.94 Screenshot of device PLABWIN10: Displaying the help of the gpresult command.</p></figcaption></figure>

#### **Task 15 - The format Command** <a href="#cn-m4-873" id="cn-m4-873"></a>

The format command allows a user to format a selected partition. Once formatted, the contents of that particular segment of the storage device are lost. Hence, this command shall be used with caution.

In this task, you will learn to use the format command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

To format the **D** drive, type the following command:

```
format d: /q
```

Press **Enter**. Notice that you are prompted for the current volume label.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-95.jpg?v=30" alt="Figure 1.95 Screenshot of device PLABWIN10: Performing a quick format of the D drive."><figcaption><p>Figure 1.95 Screenshot of device PLABWIN10: Performing a quick format of the D drive.</p></figcaption></figure>

_**Step 2**_

Type the following volume label:

```
F
```

Press **Enter**. Notice that you are prompted for confirmation.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-96.jpg?v=30" alt="Figure 1.96 Screenshot of device PLABWIN10: Entering the existing volume label."><figcaption><p>Figure 1.96 Screenshot of device PLABWIN10: Entering the existing volume label.</p></figcaption></figure>

_**Step 3**_

Type the following to proceed with formatting the D drive:

```
Y
```

Press **Enter**. Notice that you are now prompted with the volume label.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-97.jpg?v=30" alt="Figure 1.97 Screenshot of device PLABWIN10: Confirming the formatting of the D drive."><figcaption><p>Figure 1.97 Screenshot of device PLABWIN10: Confirming the formatting of the D drive.</p></figcaption></figure>

_**Step 4**_

Type the following volume label:

```
Data
```

Press **Enter**. Notice that the D drive is now formatted. Minimize the command prompt window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-98.jpg?v=30" alt="Figure 1.98 Screenshot of device PLABWIN10: Entering a new volume label."><figcaption><p>Figure 1.98 Screenshot of device PLABWIN10: Entering a new volume label.</p></figcaption></figure>

_**Step 5**_

Open the **File Explorer** from the Windows **taskbar**. In the left pane, notice that **D** drive is now labeled as **Data**.

Close **File Explorer**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-99.jpg?v=30" alt="Figure 1.99 Screenshot of device PLABWIN10: Opening File Explorer and verifying the new volume label for D drive."><figcaption><p>Figure 1.99 Screenshot of device PLABWIN10: Opening File Explorer and verifying the new volume label for D drive.</p></figcaption></figure>

_**Step 6**_

Restore the **command prompt** window from the Windows **taskbar**.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **format** command uses various parameters. To know more about these parameters, type the following command:

```
format /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-100.jpg?v=30" alt="Figure 1.100 Screenshot of device PLABWIN10: Displaying the help of the format command."><figcaption><p>Figure 1.100 Screenshot of device PLABWIN10: Displaying the help of the format command.</p></figcaption></figure>

#### **Task 16 - The copy Command** <a href="#cn-m4-915" id="cn-m4-915"></a>

The copy command allows you to copy a file from one location to another. The other location is to be specified by you, as a parameter, while issuing the command. The copy command keeps the original file as it is, and creates another instance of the file at the specified location.

In this task, you will learn to use the copy command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Let’s first create an empty text file using a command. Remember that it is easy to create a text file using Notepad but a bit tricky when you are using the command prompt.

Type the following command:

```
type NUL > ABCD.txt
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-101.jpg?v=30" alt="Figure 1.101 Screenshot of device PLABWIN10: Creating an empty text file on the command prompt."><figcaption><p>Figure 1.101 Screenshot of device PLABWIN10: Creating an empty text file on the command prompt.</p></figcaption></figure>

_**Step 2**_

To verify if the file has been created, type the following command:

```
dir
```

Press **Enter**. Notice a file named ABCD.txt is created, but it is empty.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-102.jpg?v=30" alt="Figure 1.102 Screenshot of device PLABWIN10: Listing the files in the current directory."><figcaption><p>Figure 1.102 Screenshot of device PLABWIN10: Listing the files in the current directory.</p></figcaption></figure>

_**Step 3**_

Let’s copy file named **ABCD.txt** from the current directory to **c:\Users**.

Type the following command:

```
copy ABCD.txt c:\Users
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-103.jpg?v=30" alt="Figure 1.103 Screenshot of device PLABWIN10: Copying the ABCD.txt file to c:\Users."><figcaption><p>Figure 1.103 Screenshot of device PLABWIN10: Copying the ABCD.txt file to c:\Users.</p></figcaption></figure>

_**Step 4**_

Whenever you attempt to copy a file to a destination and the same file exists, you will be prompted with a warning. If the file exists in the destination directory, you can still overwrite without getting the warning.

To do this, type the following command:

```
copy /Y ABCD.txt c:\Users
```

Press **Enter**.

The **/Y** parameter is suppressing the prompt for confirmation to overwrite a file.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-104.jpg?v=30" alt="Figure 1.104 Screenshot of device PLABWIN10: Overwriting the file by suppressing the prompt for confirmation."><figcaption><p>Figure 1.104 Screenshot of device PLABWIN10: Overwriting the file by suppressing the prompt for confirmation.</p></figcaption></figure>

_**Step 5**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **copy** command uses various parameters. To know more about these parameters, type the following command:

```
copy /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-105.jpg?v=30" alt="Figure 1.105 Screenshot of device PLABWIN10: Displaying the help of the copy command."><figcaption><p>Figure 1.105 Screenshot of device PLABWIN10: Displaying the help of the copy command.</p></figcaption></figure>

#### **Task 17 - The xcopy Command** <a href="#cn-m4-955" id="cn-m4-955"></a>

The xcopy command is used to copy the files, as well as directories, from their source location to the specified location. The specified location is a parameter, passed by the user. While copying a directory, this command copies its sub-directories as well, if present.

In this task, you will learn to use the xcopy command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To copy all text files in the current directory to the **Downloads** directory, type the following command:

```
xcopy /Y *.txt C:\Users
```

Press **Enter**. Minimize the command prompt window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-106.jpg?v=30" alt="Figure 1.106 Screenshot of device PLABWIN10: Copying all text files in the current directory to the Downloads directory using the xcopy command."><figcaption><p>Figure 1.106 Screenshot of device PLABWIN10: Copying all text files in the current directory to the Downloads directory using the xcopy command.</p></figcaption></figure>

_**Step 2**_

Open **File Explorer** from the Windows **taskbar**.

Select the **Local Disk (C:)** drive.

Right-click and click **New** > **New Folder**.

Name the new folder as:

```
 PLAB
```

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-107.jpg?v=30" alt="Figure 1.107 Screenshot of device PLABWIN10: Creating a new folder and typing in a new folder name in File Explorer."><figcaption><p>Figure 1.107 Screenshot of device PLABWIN10: Creating a new folder and typing in a new folder name in File Explorer.</p></figcaption></figure>

_**Step 3**_

Then, navigate inside the **PLAB** directory and create two directories and one text file.

Right-click and click **New** > **New Folder**.

Name the first folder:

```
Test1
```

Name the second folder:

```
Test2
```

Then, right-click and click **New** > **New Text Document**.

Name the text file:

```
PLAB
```

Close **File Explorer**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-108.jpg?v=30" alt="Figure 1.108 Screenshot of device PLABWIN10: Creating a directory, sub-directories, and a text file in File Explorer."><figcaption><p>Figure 1.108 Screenshot of device PLABWIN10: Creating a directory, sub-directories, and a text file in File Explorer.</p></figcaption></figure>

_**Step 4**_

Restore the command prompt window. You will now copy the **PLAB** directory, including empty sub-directories and text file, to the **Downloads** directory.

Type the following command:

```
xcopy c:\PLAB Downloads /e
```

Press **Enter**. Notice that the text file is now copied to the **Downloads** folder.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-109.jpg?v=30" alt="Figure 1.109 Screenshot of device PLABWIN10: Copying the PLAB directory, including empty sub-directories and text file, to the Downloads directory."><figcaption><p>Figure 1.109 Screenshot of device PLABWIN10: Copying the PLAB directory, including empty sub-directories and text file, to the Downloads directory.</p></figcaption></figure>

_**Step 5**_

To verify if the sub-directories and text file has been copied to the **Downloads** directory, type the following command:

```
dir Downloads
```

Press **Enter**.

Notice that the sub-directories and text file are now copied to the **Downloads** folder.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-110.jpg?v=30" alt="Figure 1.110 Screenshot of device PLABWIN10: Verifying if the sub-directories and text file has been copied to the Downloads directory."><figcaption><p>Figure 1.110 Screenshot of device PLABWIN10: Verifying if the sub-directories and text file has been copied to the Downloads directory.</p></figcaption></figure>

_**Step 6**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **xcopy** command uses various parameters. To know more about these parameters, type the following command:

```
xcopy /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-111.jpg?v=30" alt="Figure 1.111 Screenshot of device PLABWIN10: Displaying the help of the xcopy command."><figcaption><p>Figure 1.111 Screenshot of device PLABWIN10: Displaying the help of the xcopy command.</p></figcaption></figure>

#### **Task 18 - The robocopy Command** <a href="#cn-m4-1010" id="cn-m4-1010"></a>

The robocopy command copies file data. The necessary parameters have to be passed in the command itself such as source directory, destination directory, and file, whose contents are to get copied, etc.

Robocopy will keep the original files, and create a replica at the specified location.

In this task, you will learn to use the robocopy command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To copy the **Downloads** directory files and sub-directories to **c:\Users**, type the following command:

```
robocopy Downloads c:\Users
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-112.jpg?v=30" alt="Figure 1.112 Screenshot of device PLABWIN10: Copying the Downloads directory files and sub-directories to c:\Users."><figcaption><p>Figure 1.112 Screenshot of device PLABWIN10: Copying the Downloads directory files and sub-directories to c:\Users.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **robocopy** command uses various parameters. To know more about these parameters, type the following command:

```
robocopy /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-113.jpg?v=30" alt="Figure 1.113 Screenshot of device PLABWIN10: Displaying the help of the robocopy command."><figcaption><p>Figure 1.113 Screenshot of device PLABWIN10: Displaying the help of the robocopy command.</p></figcaption></figure>

#### **Task 19 - The net use Command** <a href="#cn-m4-1032" id="cn-m4-1032"></a>

The net use command is used to connect your computer system to the shared folder/drive on the network. Using this command, it’s possible to have the direct access to such shared directory, treating it as if it were a local directory/drive.

There are many variations of this command. Each variation allows you to determine some aspect of your connection with the folder/drive on the network.

In this task, you will learn to use the net use command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can use the **net use** command to view the existing network connection that has been mapped to a drive letter on your system.

To do this, type the following command:

```
 net use z:
```

Press **Enter**. Keep the command prompt window open.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-114.jpg?v=30" alt="Figure 1.113 Screenshot of device PLABWIN10: Viewing the existing network connection that has been mapped to a drive letter."><figcaption><p>Figure 1.113 Screenshot of device PLABWIN10: Viewing the existing network connection that has been mapped to a drive letter.</p></figcaption></figure>

_**Step 2**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. You can also map a network share or drive to a specific drive letter on your system. To do this, type the following command:

```
net use x: \\plabwin810\c$ /persistent:yes
```

Press **Enter**.

You have mapped the **x** drive of the local system with the \\\plabwin810\c$ drive. The **/persistent** parameter can have either **yes** or **no** value. The value of **yes** means that the mapping will be available when you log on to the system next time. The value of **no** means that the mapping is limited to this session only.

Minimize the command prompt window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-115.jpg?v=30" alt="Figure 1.114 Screenshot of device PLABWIN10: Mapping a network share or drive to a specific drive letter."><figcaption><p>Figure 1.114 Screenshot of device PLABWIN10: Mapping a network share or drive to a specific drive letter.</p></figcaption></figure>

_**Step 3**_

From the Windows **taskbar**, click **File Explorer**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-116.jpg?v=30" alt="Figure 1.115 Screenshot of device PLABWIN10: Opening File Explorer."><figcaption><p>Figure 1.115 Screenshot of device PLABWIN10: Opening File Explorer.</p></figcaption></figure>

_**Step 4**_

In the left pane, scroll down and verify **c$ (\\\plabwin810)** is now mapped to the drive letter **X**.

Click on the drive letter **X**. Notice its contents are displayed in the right pane.

Minimize the **File Explorer** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-117.jpg?v=30" alt="Figure 1.116 Screenshot of device PLABWIN10: Verifying the mapping."><figcaption><p>Figure 1.116 Screenshot of device PLABWIN10: Verifying the mapping.</p></figcaption></figure>

_**Step 5**_

Restore the **command prompt** window.

You will now delete the drive mapping. To do this, type the following command:

```
net use x: /delete
```

Press **Enter**. Remember that you had opened the drive mapped on **X**. Therefore, you are being prompted for confirmation for closure.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-118.jpg?v=30" alt="Figure 1.117 Screenshot of device PLABWIN10: Deleting the drive mapping."><figcaption><p>Figure 1.117 Screenshot of device PLABWIN10: Deleting the drive mapping.</p></figcaption></figure>

_**Step 6**_

You will now confirm the deletion of the drive mapping. To do this, type the following command:

```
Y
```

Press **Enter**. You are prompted with a success message.

**Minimize** the **command prompt** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-119.jpg?v=30" alt="Figure 1.118 Screenshot of device PLABWIN10: Confirming the drive mapping deletion."><figcaption><p>Figure 1.118 Screenshot of device PLABWIN10: Confirming the drive mapping deletion.</p></figcaption></figure>

_**Step 7**_

Open the **File Explorer** window.

If required, scroll down to verify the drive **X**. Notice that drive **X** does not exist anymore.

Close the **File Explorer** window.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-120.jpg?v=30" alt="Figure 1.119 Screenshot of device PLABWIN10: Verifying the drive mapping deletion."><figcaption><p>Figure 1.119 Screenshot of device PLABWIN10: Verifying the drive mapping deletion.</p></figcaption></figure>

_**Step 8**_

Restore the command prompt window. Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. The **net use** command uses various parameters. To know more about these parameters, type the following command:

```
net use /?
```

Press **Enter**. Remember that many of these parameters can be combined with the net use command.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-121.jpg?v=30" alt="Figure 1.120 Screenshot of device PLABWIN10: Displaying the help of the net use command."><figcaption><p>Figure 1.120 Screenshot of device PLABWIN10: Displaying the help of the net use command.</p></figcaption></figure>

Keep the **command prompt** window **open**.

#### **Task 20 - Use the net user Command** <a href="#cn-m4-1095" id="cn-m4-1095"></a>

The net user command allows you to perform user account-related tasks on the computer. This command allows you to create a new user, as well as modify the user account-related parameters.

This account has various parameters to it, each one of them performing a specific task. Using this command, you can manage local and domain-based user accounts.

In this task, you will learn to use the net user command.

_**Step 1**_

Ensure **PLABWIN10** is connected, and that you have the **command prompt** window open.

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To view the list of users on the local system, type the following command:

```
net user
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-122.jpg?v=30" alt="Figure 1.121 Screenshot of device PLABWIN10: Viewing the list of users on the local system."><figcaption><p>Figure 1.121 Screenshot of device PLABWIN10: Viewing the list of users on the local system.</p></figcaption></figure>

_**Step 2**_

To view the list of parameters that can be used with the net user command, type the following command:

```
net user /?
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-123.jpg?v=30" alt="Figure 1.122 Screenshot of device PLABWIN10: Viewing the help of the net user command."><figcaption><p>Figure 1.122 Screenshot of device PLABWIN10: Viewing the help of the net user command.</p></figcaption></figure>

_**Step 3**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To view the information about a specific user account on the local system, type the following command:

```
net user administrator
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-124.jpg?v=30" alt="Figure 1.123 Screenshot of device PLABWIN10: Viewing the information about a specific user account on the local system."><figcaption><p>Figure 1.123 Screenshot of device PLABWIN10: Viewing the information about a specific user account on the local system.</p></figcaption></figure>

_**Step 4**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To create a new account with the name wilson, type the following command:

```
net user wilson Passw0rd /add /times:ALL
```

Press **Enter**. Notice that you are defining the new user account name as **Wilson**.

Password is **Passw0rd**. The /add parameter adds the user account. The user is configured to log on all days of the week.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-125.jpg?v=30" alt="Figure 1.124 Screenshot of device PLABWIN10: Creating a new account named Wilson."><figcaption><p>Figure 1.124 Screenshot of device PLABWIN10: Creating a new account named Wilson.</p></figcaption></figure>

_**Step 5**_

To view the list of users on the local system, type the following command:

```
net user
```

Press **Enter**. Notice that the user account, Wilson, is now created.

_**Note:** Similar to creating a local account, you can also create a domain account by adding the /\<domain name> parameter._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-126.jpg?v=30" alt="Figure 1.125 Screenshot of device PLABWIN10: Viewing the list of users on the local system."><figcaption><p>Figure 1.125 Screenshot of device PLABWIN10: Viewing the list of users on the local system.</p></figcaption></figure>

_**Step 6**_

To delete the user Wilson, type the following command:

```
net user Wilson /delete
```

Press **Enter**.

_**Note:** If prompted for confirmation, click **Allow Access**._

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-127.jpg?v=30" alt="Figure 1.126 Screenshot of device PLABWIN10: Deleting a user named Wilson."><figcaption><p>Figure 1.126 Screenshot of device PLABWIN10: Deleting a user named Wilson.</p></figcaption></figure>

_**Step 7**_

Clear the command prompt window by entering the following command:

```
cls
```

Press **Enter**. To verify that the user account Wilson is deleted, type the following command:

```
net user
```

Press **Enter**. Notice that the user account, Wilson, is now deleted. It does not appear in the list.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-128.jpg?v=30" alt="Figure 1.127 Screenshot of device PLABWIN10: Verifying the deletion of the user named Wilson."><figcaption><p>Figure 1.127 Screenshot of device PLABWIN10: Verifying the deletion of the user named Wilson.</p></figcaption></figure>

_**Step 8**_

Close the Command Prompt window.

Click the Windows start button.

Click the user icon and then **Sign out.**

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-129.jpg?v=30" alt="Figure 1.128 Screenshot of device PLABWIN10: Showing the option for Sign out."><figcaption><p>Figure 1.128 Screenshot of device PLABWIN10: Showing the option for Sign out.</p></figcaption></figure>

#### **Task 21 - Commands available with standard privileges vs. administrative privileges** <a href="#cn-m4-1159" id="cn-m4-1159"></a>

Commands are divided into two segments. The first type of commands run with standard privileges, and the second type of commands need administrative privileges to run. Commands running with administrative privileges are used to change the system functionality and therefore, if not used with caution can make a system non-functional.

In this task, you will learn to use the commands with standard vs. administrative privileges.

_**Step 1**_

For this task, you will need to firstly disable **server auto login** and then click back on the **exercise content** tab to proceed.

Ensure that you are logged into the **Practice Labs** environment. Click **Access your settings** tab, which is the **cog** icon in the toolbar.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-130.jpg?v=30" alt="Figure 1.129 Screenshot of Practice Labs Environment: Clicking Access your settings, which is the cog icon."><figcaption><p>Figure 1.129 Screenshot of Practice Labs Environment: Clicking Access your settings, which is the cog icon.</p></figcaption></figure>

_**Step 2**_

In the left pane, under the **Device** section, notice that **Server auto login** is enabled.

Click on the slider to disable it.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-131.jpg?v=30" alt="Figure 1.130 Screenshot of Practice Lab Environment: Clicking on the left side of the slider of the Server auto login."><figcaption><p>Figure 1.130 Screenshot of Practice Lab Environment: Clicking on the left side of the slider of the Server auto login.</p></figcaption></figure>

_**Step 3**_

Notice that the **Server auto login** is now disabled.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-132.jpg?v=30" alt="Figure 1.131 Screenshot of Practice Lab Environment: Showing the Server auto login as disabled."><figcaption><p>Figure 1.131 Screenshot of Practice Lab Environment: Showing the Server auto login as disabled.</p></figcaption></figure>

_**Step 4**_

Ensure that you have powered on the required devices.

Connect to **PLABWIN10**.

_**Note:** If you were previously connected to PLABWIN10, you might already be logged in. Please log out of the administrator user._

Select the **Other user** option as shown in the below image and type the following user name:

```
jan.regus
```

In the password field, type the following:

Passw0rd &#x20;

Click the **Submit** button. Alternatively, press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-133.jpg?v=30" alt="Figure 1.132 Screenshot of device PLABWIN10: Logging on to the system as jan.regus."><figcaption><p>Figure 1.132 Screenshot of device PLABWIN10: Logging on to the system as jan.regus.</p></figcaption></figure>

_**Step 5**_

In the **Type here to search** textbox in the taskbar, type the following command:

```
command prompt
```

Under the **Best Match** section, select **Command Prompt**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-134.jpg?v=30" alt="Figure 1.133 Screenshot of device PLABWIN10: Opening the command prompt."><figcaption><p>Figure 1.133 Screenshot of device PLABWIN10: Opening the command prompt.</p></figcaption></figure>

_**Step 6**_

Let’s execute the **ipconfig** command in the standard mode. It will show its corresponding output.

Type the following command:

```
ipconfig
```

Press **Enter**.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-135.jpg?v=30" alt="Figure 1.134 Screenshot of device PLABWIN10: Running the ipconfig command."><figcaption><p>Figure 1.134 Screenshot of device PLABWIN10: Running the ipconfig command.</p></figcaption></figure>

_**Step 7**_

Now, let’s try the **sfc** command, to see if it works in this standard mode. Type the following command:

```
sfc
```

Press **Enter**. Notice that you are prompted to run this command with administrative privileges.

<figure><img src="https://www.practice-labs.com/authenticated/images/220-1002/image-m4-c-136.jpg?v=30" alt="Figure 1.135 Screenshot of device PLABWIN10: Running the sfc command and displaying error."><figcaption><p>Figure 1.135 Screenshot of device PLABWIN10: Running the sfc command and displaying error.</p></figcaption></figure>

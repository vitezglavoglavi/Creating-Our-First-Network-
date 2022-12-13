# 
Creating Our First Network - Exercise - Cisco Packet Tracer

Packet Tracer is a simulation tool that will let us build network models, experiment with network behaviour, and ask “What if” questions. As a cybersecurity analyst, we will use Packet Tracer to understand, investigate, and escalate network issues. In this lab, we will learn how to design a network, connect wired and wireless devices.




Wired Network Design

We’ll start building our network in this step. To build a network, we must first implement devices that will communicate with one another soon. The devices we need for this step: 1 PC, 1 laptop, 1 printer, and 1 switch 2960
1.	Click on the “End Devices” icon on the “Device-type” selection box
2.	Click on the “End Devices” icon on the bottom menu
3.	Go to the “Device-specific” selection box and select the PC
4.	Click on the workspace.

The Packet Tracer provides a default name to the devices. By clicking on the name, we can rename the devices, which is very helpful in managing the network appropriately.
Renaming the PC from PC0 to PC1:
1.	Double-click on the default name “PC0”
2.	Change it to “PC1”

PC 2 Selection:
1.	Click on the “End Devices” icon on the “Device-type” selection box
2.	Click on the “End Devices” icon on the bottom menu
3.	Select the laptop on the “Device-specific” selection box
4.	Click on the workspace
5.	Rename the device “PC2”, with the same steps used for PC1

Printer Selection:
1.	Click on the “End Devices” icon on the “Device-type” selection box
2.	Click on the “End Devices” icon on the bottom menu
3.	Go to the “Device-specific” selection box and select the printer
4.	Click on the workspace
5.	Rename the device “Printer1”

Network device (switch) selection
1.	Click on the “Network Devices” icon on the “Device-type” selection box
2.	Click on the “Switches” icon on the bottom menu
3.	Go to the “Device-Specific” selection box and select “Switch 2960”
4.	Click on the workspace
5.	Rename the device “S1”


![1](https://user-images.githubusercontent.com/120283135/207422535-1fe949dc-54b7-408a-b76b-d3da81336f41.png)

Connecting PC2 to S1:
1.	Select the “Connections” icon on the “Device-type” selection box    
2.	Select the same icon on the bottom menu
3.	Select “Black Copper straight-through” cable on the “Device-specific” selection box.    
4.	Click on PC2
5.	Select the interface “FastEthernet0”
6.	Drag the cable to S1 and click on it
7.	Select the interface Fastethernet0/1, and the connection will be established

Connecting PC1 and Printer1 to S1:
Notice: For all the devices, use the same process for connections
1.	Connect PC1 to S1:
For PC1, select the interface FastEthernet0
For S1, select the interface Fastethernet0/2/
2.	Connect Printer1 to S1:
For the printer1 select the interface FastEthernet0
For S1, select the interface Fastethernet0/3

![image](https://user-images.githubusercontent.com/120283135/207428019-ca666364-68b5-48ba-a560-087ea8c26804.png)

Connect Wireless Devices:
In the previous steps, we connected wired devices. Now we’ll apply the same principles to wireless devices.
The devices used in this step are 1 Access Point, 1 Smartphone, and 1 Laptop.
1.	Click on the “Network Devices” icon on the “Device-type” selection box
2.	Click on the “Wireless Devices” icon on the bottom menu
3.	Go to the “Device-specific” box and select the “AP-TP”
4.	Click on the workspace

Select the END Device (smartphone):
1.	Click on the “End Devices” icon on the “Device-type” selection box
2.	Click on the “End Devices” icon on the bottom menu
3.	Go to the “Device-specific” selection box and select the “Smart Device”
4.	Click on the workspace. The connection will be automatically established.

![image](https://user-images.githubusercontent.com/120283135/207426994-8c418ef2-4726-43f3-9859-5016c8899176.png)

Select the laptop:
1.	Click on the “End Devices” icon on the “Device-type” selection box
2.	Click on the “End Devices” icon on the bottom menu
3.	Select the laptop on the “Device-specific” selection box
4.	Click on the workspace
5.	Rename the device “PC3” and place it near the access point

We’ll now change the laptop’s network to integrate it into our network.
Turning off the laptop and changing the network:
1.	Click on PC3
2.	Click on the power button (2) to shut down the machine. As soon as you do, the light just under the button will turn off
3.	Change the laptop’s network card. Click and maintain the network interface (3)
4.	Drag and drop it in the yellow area (4)
5.	Add the wireless card WPC300N by dragging and dropping it to the location of the previous network card (3)
6.	Turn on the machine and click on the power button

Now we would verify if the laptop connected to the Wi-Fi:
1.	Close the windows
2.	The laptop should connect automatically to the Wi-Fi

![image](https://user-images.githubusercontent.com/120283135/207424173-be75e7a2-2366-42c5-9f30-f29115de2b23.png)

Configure the PCs with IP addresses
After configuring the network and establishing connections between the devices, we’ll need to configure them by assigning them IP addresses, which are required for network communication. We’ll begin with PC1.

Configuring PC1:
1.	Click on PC1
2.	Click on the “Desktop” tab
3.	Click IP Configuration
4.	Enter the IP address or PC1, which is 192.168.1.1
5.	Enter the subnet mask, which is 255.255.255.0
6.	Close the windows

![image](https://user-images.githubusercontent.com/120283135/207424346-b60892da-b183-4918-b0da-42d5681a7399.png)

Configure PC2:
1.	Click on PC2, and then click on the “Desktop” tab
2.	Click on the IP Configuration
3.	Enter the IP address 192.168.1.2
4.	Enter the subnet mask 255.255.255.0

![image](https://user-images.githubusercontent.com/120283135/207424405-a355f4cd-4aa4-4e02-aad4-ffa9955c5ea1.png)

Configure the PCs with IP Ping command:
1.	Click on PC1
2.	Click on “Command Prompt”
3.	Send “ping” to PC2

![image](https://user-images.githubusercontent.com/120283135/207424452-9af4be6d-f5ee-4677-8b06-d7b5ce75df87.png)


The response shows the IP address and the size of the packets being sent on the first line. The next four lines show the replies form each individual packet, including the time (in milliseconds) it took for the response and the time-to-live (TTL) of the packet. TTL is the amount of time that must pass before the packet is discarded. At the bottom, you’ll see a summary that shows how many packets were sent and received, as well as the minimum, maximum, and average response time.

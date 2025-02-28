FTP Server Configuration in Cisco Packet Tracer
Introduction
This guide explains how to set up and configure an FTP (File Transfer Protocol) server in Cisco Packet Tracer. FTP is a widely-used protocol for transferring files over a network. By setting up an FTP server in Packet Tracer, you can simulate file uploads and downloads between network devices.

Prerequisites
Cisco Packet Tracer installed on your machine.
Basic knowledge of networking and TCP/IP protocols.
A Packet Tracer project with a network topology.
Steps to Configure an FTP Server
1. Add the FTP Server
Open Cisco Packet Tracer and create a new project.
Add a Server:
From the End Devices section in the device palette, drag and drop a Server onto the workspace.
A server icon will appear on the workspace.
2. Configure the FTP Service on the Server
Access the Server Configuration:

Click on the Server icon to open the configuration window.
In the server configuration window, go to the Config tab.
Enable the FTP Service:

In the Global Settings section, you'll see different services such as HTTP, DNS, FTP, and others.
Select the FTP option from the list.
Check the Enabled box to activate the FTP service.
Set the FTP Directory:

Under the FTP settings, you can configure directories where files will be stored.
You can create folders for different types of files (e.g., /shared/, /uploads/, etc.).
Add files to the FTP server by clicking Add File and uploading the file(s) from your local machine to the FTP server.
Set FTP Username and Password (Optional):

For security purposes, it's good practice to set a username and password for accessing the FTP server.
Under the FTP tab, set the Username and Password for the FTP service.
Example:

Username: admin
Password: password123
3. Configure the Client (PC or Laptop)
Add a Client Device:

From the End Devices section, drag and drop a PC or Laptop onto the workspace.
Configure the Client IP Address:

Click on the PC or Laptop to open its configuration window.
Go to the Desktop tab and select IP Configuration.
Assign a Static IP Address to the device and configure the subnet mask and default gateway (if required).
Example:

IP Address: 192.168.1.2
Subnet Mask: 255.255.255.0
Gateway: 192.168.1.1 (if using a router)
Configure FTP on the Client:

In the Desktop tab of the client, open the FTP application.
In the FTP window, enter the IP address of the FTP server (e.g., 192.168.1.1).
If prompted, enter the Username and Password you set earlier in the FTP server configuration.
4. Testing the FTP Configuration
Test Connection
Ping the FTP Server:
On the client device, open the Command Prompt from the Desktop tab.
Type ping <FTP_SERVER_IP> (e.g., ping 192.168.1.1).
If the ping is successful, it indicates the client can reach the FTP server.
Upload/Download Files
Upload Files to the FTP Server:

On the client, open the FTP application from the Desktop tab.
Log in using the FTP server's IP address, username, and password.
Browse the directories, and select a file from your local machine to upload to the FTP server.
Click Upload to transfer the file.
Download Files from the FTP Server:

In the FTP application, browse the directories on the FTP server.
Select a file to download and click Download to transfer the file to the client device.
Verify File Transfer
On the FTP server, open the Config tab and check the FTP settings.
Verify that the uploaded or downloaded files appear in the corresponding directories.
5. Troubleshooting
Unable to Connect: Ensure that the client device has the correct IP address and subnet mask. Make sure the FTP server is reachable by using the ping command.
Authentication Errors: Double-check the username and password set for the FTP server.
File Transfer Issues: Ensure that the client has the appropriate permissions to upload and download files from the FTP server.
Conclusion
You have successfully configured an FTP server in Cisco Packet Tracer, enabling file transfers between devices on the network. FTP is a useful protocol for transferring files and can be simulated easily within Packet Tracer for testing and educational purposes

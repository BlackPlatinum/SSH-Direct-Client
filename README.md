# <img src="https://i.postimg.cc/QtghNf7w/icon.png" width="50" /> SSH-Direct-Client 
WPF-Based Windows-Only Software Providing Secure Proxy Tunnel to A Remote Server

## Introduction
This Software is capable of creating a secure tunnel to a remote server and share it on a dynamic local port. The software acts like __ssh -L__ command in Terminal but in a much more simple and user-friendly way.
In the process of making this software, Renci's <a href="https://github.com/sshnet/SSH.NET">SSH.NET</a> was used and altered a bit to match this software's needs. 

## System Requirements

<strong>Software:</strong>
- This software supports Windows 10 (x64) version 20H1 and later. (Older versions are not guaranteed to run this app but you are welcome to try the binaries provided in assets of each release.)
- This software uses <a href="https://dotnet.microsoft.com/en-us/download/dotnet/6.0">.Net 6</a> which is integrated in the app and DOES NOT require installation. However, in future a stripped version will be released which does not contain .Net 6 Runtime and takes less disk space.

<strong>Hardware:</strong>
- Client app does not require a high-end system. If your system is capable of running Windows 10, it definitely can run this app.
- Make sure your display resolution is high enough. In lower resolutions, the app might look cropped so you have to collapse some of the expanders to see contents that reside on the bottom of the app.

## Instructions
Instruction of each part is provided in the same order of their placement from top to bottom on app interface.

### 1) Connection Info
1- Fill in the Host Address in correct format (e.g. 123.123.123.123)<br/>
2- Default Host Port for SSH is 22. If your server communicates through another port, replace it with the default value.<br/>
3- The Username and Password, provided by the server must be entered correctly in order to connect to host.<br/>

### 2) Connect Button
Connect button is a simple button for either connecting or disconnecting from the host server. The button also represents the connection state in the following manner:<br/>
1- Green Color and Spinning : Connecting to host<br/>
2- Green Color and Still: Successful connection to host<br/>
3- Yellow Color and Spinning: An error has occurred and client is reconnecting<br/>
4- Red Color and Still: An error has occurred which keeps client from connecting to host<br/>

### 3) SOCKS5 Properties
As mentioned earlier, the client shares the tunnel to a SOCKS5 dynamic local port.<br/>
The default value for SOCKS5 IP Address is 127.0.0.1 (also known as localhost) and the default value for SOCKS5 port is 1080. This gives you the ability of configuring other apps in order to use this tunnel through 127.0.0.1:1080 address. You can override these fields to achieve your own desired address.

### 4) SSH Connection Properties
Here you can set parameters for SSH connection or leave them be. It is recommended to leave them at default values which is 0.

### 5) Extra Properties
For now, the only option provided in this section is Switch Theme ability. You can use Dark or Light mode to match the app to your own style.

### 6) Logs
This section displays connection log, essential for debugging and fixing connectivity problems and issues.

## Conclusion

The client is easy to install and use. If you face any problems or bugs, related to app itself or the installer, feel free to report it.

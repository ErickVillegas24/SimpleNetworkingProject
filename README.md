<h1>Simple CISCO Packet Tracer Networking Project</h1>

<h2>Description</h2>
Designed and simulated a Simple Network System using CISCO Packet Tracer.
<br />


<h2>Utilities Used</h2>

- <b>CISCO Packet Tracer Version 8.2.1<b>

<h2>Program walk-through:</h2>

<p align="center">
Place (1) 2911 Router and (2) 2960-24TT Switches. Label the left Switch "ACCOUNTS" and the right Switch "DELIVERY" <br/>
<img src="https://i.imgur.com/HyXWi72.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Place (2) PCs and (1) Printer for each switch. Connect each device using the "Automatic" cable type<br/>
<img src="https://i.imgur.com/ViNN4jT.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Visually Separate the Network by placing (2) different colors for each switch/side: <br/>
<img src="https://i.imgur.com/wQMQNKE.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Conduct subnetting and obtain least amount of IPs possible, while still being able to assign an IP for each device <br/>
<img src="https://i.imgur.com/Ll2CaIl.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Layout the IPs and see how many are available and what needs to be reserved:  <br/>
<img src="https://i.imgur.com/Q05l9Xx.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Place IPs in their respective locations:  <br/>
<p align="center">
- Accounts = 192.168.40.1 - 8 (Gig0/0)
<br />
- Delivery = 192.168.40.9 - 15 (Gig0/1)
<img src="https://i.imgur.com/G4OqXSq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the Router and the "CLI" or Command Line Interface Tab and enter the following to enable and configure the router:  <br/>

- <b>"En"<b>
- "Config T"
- "Int Range Gig 0/0-1"
- "No Shutdown"
- "Do Wr"
<p align="center">
<img src="https://i.imgur.com/nztsvHZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once the router displays the green arrows stating it's in an "UP" state, we need to assign each side their IP ranges. The following information will be inputted:  <br/>

- <b>"exit"<b>
- "int gig 0/0"
- "ip address 192.168.40.1 255.255.255.248" (This will be assigned to the "Accounts" section)
- "int gig 0/1"
- "ip address 192.168.40.9 255.255.255.248" (This will be assigned to the "Delivery" section)
- "do wr"
<p align="center">
<img src="https://i.imgur.com/MKjCfSM.png" height="80%" width="80%"
<br />
<br />
<br />
Pending.....
<p align="center">
- <b> WHATS NEXT: Will be assigning IPs to each device and conduct "Ping" within the Command Prompt to confirm Network travel across different subnets. </b>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

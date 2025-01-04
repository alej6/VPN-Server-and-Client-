# VPN-Server-and-Client-

<h2> Overview</h2>
This repository serves as a writeup for a project assigned for ITC2200 Networking Foundations. This project focuses on creating a Virtual Private Network (VPN) server and client using OpenVPN. The goal was to ensure secure and encrypted connections between the client and server. 

<h2> Video Demonstration </h2>
<p>You can watch the demonstration of the VPN server setup here:</p>
<a href="https://drive.google.com/file/d/1injukQ2l1pGyveb9IAF2f33UWkIM03qk/view?usp=share_link" target="_blank">
     VPN Server Setup Video
</a>


<h2> Project Details </h2>
<p> Creating the VPN server and client involved several steps which included installing OpenVPN on an Ubuntu VM, creating and configuring necessary files, and troubleshooting common issues.
 </p>
<ul>
  <li> <strong>VPN Server Setup:</strong>  The server was configured by installing OpenVPN, creating a configuration file (`server.conf`), and enabling the server to run at startup using `systemctl`.</li> 
  <li> <strong> VPN Client Setup:</strong> The client was configured by creating a `client.ovpn` file with the server address, port, and certificate paths, followed by importing it into the OpenVPN client software for a successful connection. </li>
</ul>

<h2> Challenges Encountered</h2>
<ul>
  <li>Missing files (e.g., `dh.pem`, `server.crt`) were identified and created.</li>
  <li> Incorrect file permissions were resolved using the `chown` command.</li>
  <li> Configuration errors in `server.conf` were corrected using manual testing commands like `openvpn --config /etc/openvpn/server/server.conf`.</li>
</ul>

<h2> Takeaways</h2>
<ul>
  <li><strong>Attention to detail: </strong> Small configuration errors can lead to issues with the VPN functionality</li>
  <li><strong> The power of logs: </strong> Logs proved to be an essential tool for diagnosing and resolving issues.</strong></li>
  <li><strong> Security best practices: </strong> Separating the VPN server and CA enhances security and simplifies management in production environments.</strong> </li>
  <li><strong> PKI: </strong> Understanding the role of PKI in authenticating and securing communications was crucial for setting up the VPN. </li>
</ul>

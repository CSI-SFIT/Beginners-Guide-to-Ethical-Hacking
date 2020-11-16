# Maintaining access

 Once a pentester manages to gain access to the target system, he should work hard to keep his boat afloat, metaphorically speaking. He can choose either to use the hijacked system as a launching-pad (i.e. to be part of a botnet for DDoS attacks or spam campaigns), at this moment attack, scan and exploit other systems, or keep on exploiting the current system in stealth mode. Both actions can entail a great deal of damage.

## Tools and Methods for Maintaining Access

  A backdoor or a Trojan is a convenient tool for establishing easy access into the already breached system. A Trojan horse provides access at the application level, but to gain it, the user needs to install the piece of malware locally. In Windows-run systems, the majority of Trojans proceed to install themselves as a service and then run as a local system, having administrative access. Furthermore, the pentester can mount Trojans to sneak out passwords, credentials, and any other sensitive information stored on the system.
  
  Much like remote access Trojans (RATs), backdoors are installed in target systems and come with built-in upload/download functionality. They upload gathered files of interest and then rely on ports like port 53 (for DNS) and 80 and 443 (for HTTP and HTTPS, respectively) to cover up their traffic. TrendMicro reports cyber incidents connected to attackers bypassing “the connection restriction whenever they use HTTP to transmit data and to bypass detection. Based on [TrendMicro’s] investigation, there are instances when attackers manually download the .ZIP file containing all collected data.”
 
### Covert Channel

 A covert channel is when data is being sent through secret communication tunnels. VoIP, DNS tunnels, ICMP tunnels, and HTTP tunnels are such paths for data extraction from the inside of a network. All of these covert channels can transport encrypted data as well.

 Although detecting covert channels is not impossible, it may require considerable efforts on the part of the victim. Network signatures, flow data analysis and protocol analysis are some of the indicators of anomalies in the outbound traffic which a pentester wielding the right tools can come across. On top of that, despite that protocol- or application-specific tools do not yield easily to security purposes, they could show better results in comparison to their security-specific counterparts.

 To detect a covert tunnel is one thing, but to block it is a completely different matter. Pentester can:

 - Block ICMP outbound at the corporate information border;

 - Block DNS requests to servers outside the corporate network but not to such to internal DNS servers;

 - Leverage Web proxies to dispose of the HTTP tunnels;

 Delay delivery for a voicemail in cases of VoIP RTR exfiltration tunneling so that he can send to an audio processor, which will examine every packet for encoded data in a voicemail (in a similar fashion as antispam software works).

---

### Rootkit

 A rootkit is a type of malware highly adept at hiding itself from a computer system. Hence, what distinguish rootkits from other types of malware is their heightened ability to conceal themselves to bypass the computer security measures. In effect, that is the main idea behind their creation.

 Rootkits are usually loaded with the help of Trojan horses, starting on the targeted platform with “user” level access. Once getting an initial foothold into the system under attack, they spy on passwords and other similar login details to gain “administrator” level access. This process is called privilege escalation. Nevertheless, the rootkits’ real “specialty” is maintaining access.

 Unlike the ordinary viruses which attempt to inflict as much damage as possible for a short period, rootkits tend to lurk in the targeted system, progressively and slowly undermining it. Prima facie the emphasis is on the word ‘secrecy’. For example, rootkit keyloggers are designed to record the words the victim types without his knowledge. It has plenty of time to steal sensitive information given the fact that this malware may remain undetected, which will, in turn, increase the probability of identity theft.

---

### Data Exfiltration

 Data exfiltration is an unauthorized transfer of data from a computer system or IT servers to an external system or device. It can be carried out manually (similar to a ‘copy-paste’ command) or automatically via malware spread across a network.

 When the data is exfiltrated electronically, it is usually through different kinds of web protocols, tunneling protocols, email or file transfers. While the file transfer protocol (FTP) is regarded as a standard network protocol whose purpose is to transfer files, it may also be used to facilitate data exfiltration campaigns. Other protocols and techniques are applicable as well, for instance, routing control packets, secure shell, peer-to-peer, instant messaging, Windows Management Instrumentation, hiding data within video or images, and VoIP. Webcams, microphones, and similar peripheral devices may be rigged to monitor the target’s activities. Pentester can also make use of HTTP file transfers or the Tor anonymity network as a means to mask location and traffic.

 Sometimes before the exfiltration takes place, the pentester would want to process the data to transfer it easier outside the exploited system. Typical activities with relation to this point are compression, encryption and password protection. Then the processed data will be uploaded from within the target network to a server somewhere outside. Common traffic channels are a preferable route for smuggling data out of the targeted system since the extraction will blend in with the noise of the network.

 The FrameworkPOS malware is an excellent illustration of how data exfiltration works – it leverages memory scraping techniques to dig out credit card information stored somewhere in processes running on the endpoint. Upon finding the relevant data, the malicious software performs DNS tunneling to connect to a command and control server to pull out the data. Furthermore, the FrameworkPOS encodes via XOR the credit card information, hostname and IP address, and adds the encoded package to an HTTP request to export data from the environment. This trick effectively obfuscates a firewall- and proxy-based inspection.

 Undetected data exfiltration is what wrongdoers are looking for in many cases, as the real-life cyberattacks against Target and Home Depot demonstrate. This is so because some of the information they steal is secret, and it is more valuable or only valuable when it stays secret.


 Metasploit is the widely and most reliable tool for this task refer [Here](https://www.javatpoint.com/methods-to-maintain-access) to get practical.

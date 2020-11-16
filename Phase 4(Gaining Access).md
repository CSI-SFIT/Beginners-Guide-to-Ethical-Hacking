# Gaining Access
 
  Gaining access is the most important phase of an attack in terms of potential damage, although attackers don’t always have to gain access to the system to cause damage. For instance, denial-of-service attacks can either exhaust resources or stop services from running on the target system. Stopping a service can be carried out by killing processes, using a logic/time bomb, or even reconfiguring and crashing the system. Resources can be exhausted locally by filling up outgoing communication links.

  The exploit can occur locally, offline, or over a LAN or the Internet as a deception or theft. Examples include:

    Stack-based buffer overflows
    Denial-of-service and distributed denial-of-service
    Session hijacking

  Attackers use a technique called spoofing to exploit the system by pretending to be strangers or different systems. They can use this technique to send a malformed packet containing a bug to the target system in order to exploit vulnerabilities. Packet flooding may be used to remotely stop availability of the essential services. Smurf attacks try to elicit a response from the available users on a network and then use their legitimate address to flood the victim.

  Factors that influence the chances of an attacker gaining access into a target system include the architecture and configuration of the target system, the skill level of the perpetrator, and the initial level of access obtained. The most damaging type of the denial-of-service attacks can be distributed denial-of-service attacks, where an attacker uses zombie software distributed over
  several machines on the Internet to trigger an orchestrated large scale denial of services.
 
# Stack-based buffer overflows
  
  The Buffer Overflow is one of the oldest vulnerabilities known to man. It can be tracked all the way back to the late 80s, when the self-propagating Morris Worm wreaked havoc. Modern applications implement virtual memory fundamentals, unlike physical memory addresses in old times. When virtual memory is 
  used, application code and the processor make use of virtual memory addresses. In other words, the OS and the chipset work in sync to map and coordinate between virtual and physical memory addresses.
  
  The temporary storage areas in the memory are also known as buffers. When the application can be tricked (usually due to coding errors) into storing more data than the buffer can hold, it overflows into adjacent buffers. This Buffer Overflow can lead to a wide range of issues, including data corruption, segmentation faults, exceptions and more.
  
  The probability of this vulnerability differs from language to language, but C, C++ and Assembly are considered most susceptible due to their outdated memory management capabilities. Advanced hackers can initiate Buffer Overflows with specially crafted malicious payloads to cause application crashing, data theft or even give them remote access.
  
  Click [Here](https://blog.rapid7.com/2019/02/19/stack-based-buffer-overflow-attacks-what-you-need-to-know/) to know more.
  
# Denial-of-service
  
  Denial of service (DoS) attacks are one of the major security challenges in the developing cloud computing models. DoS is a security threat that occurs when an attacker prevents appropriate users from accessing specific devices, computer system, or other IT resources in the cloud.
  
  DoS attacks are simple but successful and can cause extreme damage to the cloud resources and services and often they target the computer networks’ bandwidth or connectivity. With one attack, an organization’s cloud security can be affected for days or even weeks and the servers could become unavailable to other devices and users throughout the network.
  
## Different Method of DoS Attacks
 
   DoS attacks come in different categories such as: bandwidth attacks, connectivity attacks, process disruption, physical disruption and data corruption.
   
   The most common method of attacks, Flooding services, occurs when the cloud network gets flooded with traffic by receiving several requests at once and getting overloaded, causing the server to slow down and eventually stop responding. Buffer overflow attack is a software coding mistake that an attacker uses by sending more traffic to a network address to gain access to the system.
   
   ICMP flood, also known as smurf attack or ping of death, effects misconfigured network devices by attacking when the system receives too many ICMP ping commands. Another attack, SYN flood also known as half-open attack, repeatedly sends a request to connect to a targeted server machine to overwhelm all open ports, but never completes the handshake, causing the targeted server to poorly respond or not respond at all.
    
   Click [Here](https://www.rapid7.com/fundamentals/denial-of-service-attacks) to know more.
 
# Session hijacking

  Session hijacking is when an attacker takes over a TCP session between two machines, quite often in midstream, and usually for the purposes of either stealing information or disrupting or inhibiting the flow of information.
  Because authentication only occurs at the start of TCP session, an attacker can use captured, brute –force, or a reverse-engineered session ID to seize control of a legitimate user’s Web application session while the session is still in progress.
  A session ID is an identification string (usually a long, random, alphanumeric string) that is transmitted between the client and the server. 
  Session IDs are commonly stored in cookies, URLs, and hidden fields of Web pages. 
  
  There are several problems with session IDs.In blind hijacking, the attacker injects such data as malicious commands into intercepted communications between two hosts commands such as "net.exe localgroup administrators EvilAttacker".It is called blind hijacking because the attacker can only inject data into the communications stream, he or she cannot see the response to that data (such as the command completed successfully).
  
  In a session theft attack, the attacker neither intercepts nor injects data into existing communication between two hosts. The attacker creates new sessions or uses old ones. This type of session hijacking is most common at the application level, especially Web applications.
  
  Session hijacking at the network level is especially attractive to attackers. They don't need host access, as they do with host-level session
  hijacking. Nor do they need to customize attacks on a per-application basis, as they do at the application level. Network-level session-hijacking 
  attacks allow attackers to remotely take over sessions, usually undetected.
  Successfully hijacking a session at the network level requires an attacker to overcome various obstacles.
  
  Click [Here](https://www.rapid7.com/db/vulnerabilities/drupal-cve-2014-9015) to know more.
   
  The practicals for this attacks isn't shown here as teaching their practicals is only for those who can responsibly handle it.
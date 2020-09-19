# Information Gathering
  How does a common penetration test start? First, we need to determine the pentest area, set specific goals and objectives. Naturally, 
 preparations take most of the project time. After all, the goal of a pentest is not only to detect a known software vulnerability. Nor
 we strive to find all the gaps in IT infrastructure using automated scanners, which are utterly useless. But that would be a story for
 a different blog post. Pentesting is a complex multi-step process, and surveillance plays here a key role. After all, the main goal of
 a pentest is to mimic the real actions of the intruders.The result of our pentesting session depends on the completeness of the 
 information we gather. Recon is the most important and the longest stage of pentesting, as we will build attack vectors at the detected
 entry points based on the information we gathered previously. All the data we obtain in the process will be included in our final report.  

  This divides this phase into two parts:-

 1.Active information gathering requires direct interaction with the target system. At this stage, we obtain information about the open
  ports, services, versions of applications, CMS, version of the OS, list of applications hosted on non-standard ports, etc. Most widely
  used tools for recon are Nmap and Red Hawk.

 2.Passive information gathering allows receiving data from various open sources: Whois domain names, social networks, employees data,
  mapping nodes, second-level domains test applications and hosts, mail servers, list of applications hosted on the same IP address, 
  address space and other open information. Search engines, such as Google,  Shodan, Pastebin, and others, can bring some good results here.
 
  # How To Conduct Active Recon / Active Information Gathering
  
  For this purpose we will be using Nmap and it is probably the most well-known tool for active network reconnaissance. Nmap is a network 
  scanner designed to determine details about a system and the programs running on it. This is accomplished through the use of a suite of 
  different scan types that take advantage of the details of how a system or service operates. By launching scans against a system or a range 
  of IP addresses under a target’s control, a hacker can learn a significant amount of information about the target network.
  This tool is pre-installed in Kali Linux and it is an command-line based tool. It also has an userfriendly UI version named as Zenmap which we 
  can use on linux as well as windows and for windows users we will be using Zenmap instead of Nmap since the only difference lies is Zenmap has 
  a GUI where nmap is commandline based both are same in functioning and provides most accurate results.
 

 # Installing Nmap/Zenmap On  A Windows Machine
  
  1.Browse to https://nmap.org/download.html and download the latest self-installer.
  
  2.Run the downloaded .exe file. In the window that opens, accept the license terms.
 
  3.Choose the components to install. By default, the Zenmap GUI will be installed. (If we uncheck the GUi then we will have Nmap and if we dont
    we will have Zenmap)
 
  4.Select the install location and click Install.
 
  5.The installation should be completed in a couple of minutes and then we would be ready to start our recon.
  
  
  # Getting Started
  Open terminal and let's get started with this. Windows users will get the option to run scans as the name of scans are mentioned in Zenmap where for nmap users commandline is provided.
  
  A TCP Connect Scan, we can find which ports are open on each host. Recall that a TCP Connect scan creates an established TCP connection
  with the target by completing the TCP three-way handshake.
  This is done by Running nmap -sT on each host(commandline ).
  
  There are features that will allow the Nmap tool to perform one or even all of the following alternatives. By using –osscan-limit for OS detection results with too many possible matches, the Nmap tool will limit match results to the best possible OS of the target host. If, on the other hand, the results do not yield a perfect match, a user may use the "–osscan-guess" command.
  
  These two were just an example showing how nmap  works you can discover many other with the help of cheat sheet provided. Do it on your own network moniter the users and also on any host. With Nmap, we can discover what hosts and services are up and running on a network, but there are dozens of other characteristics but only if you own that or you have a permission because even peformining reconnaissance is illegal on any third party network without the consent as it may leak out open ports which can futher be misued by the hackers/individual .
  
  
  video tutorial:- Comming soon 
  
  ## Resources
 
  Nmap offical site :-https://nmap.org/download.html

  Nmap cheat sheet:- https://www.stationx.net/nmap-cheat-sheet/
  
  
  FOR any queries contact via mail on harmhacker@protonmail.com
  
  
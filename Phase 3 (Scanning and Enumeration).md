# Scanning and Enumeration
   The initial objectives and requirements forperforming scanning and enumeration in support of a penetration test or vulnera-bility 
  assessment. This includes discussing the final phase of reconnaissance,vitality. After that, we will dig into some scenarios in which 
  you will see how youcan use these different tools and techniques to their full advantage. Last, we’ll doa hands-on challenge so you can 
  test your new (or refined) skills in a real-world scenario.
  
  In a penetration test, there are implied boundaries. Depending on the breadth andscope of your testing, you may be limited to testing a
  certain number or specific typeof host, or you may be free to test anything your client owns or operates.
  
 ![](https://nmap.org/images/sitelogo.png)
 
 For this purpose also our main tool used would be nmap.I hope you guys have refered to the cheat-sheet provided in previous phase.
  
  # USAGE
  
  nmap [Scan Type(s)] [Options] Target(s)
  [Scan Type] is the type of scan to perform. Different scan options are available and arediscussed throughout this chapter.
  
  [Options] include a wide variety of configuration options including DNS resolution, use oftraceroutes, and more.
  
  Target is the target specification which can be a single host, a list of host names or IPs,or a full network.
  
  example 
  root@HARM:~/nmap_scans# nmap -sn --send-ip 192.168.1.0/24 -oA
  
  nmap-sweep
  
  Starting Nmap nmap-7.80-1 at 2020-09-29 16:17 IST
  
  Nmap scan report for 192.168.1.1
  
  Host is up.
  
  Nmap scan report for 192.168.1.100
  
  Host is up (0.061s latency).
  
  MAC Address: 00:0C:29:XX:XX:XX (VMware)
  
  Nmap scan report for 192.168.1.110
  
  Host is up (0.0047s latency).
  
  MAC Address: 00:0C:29:XX:XX:XX (VMware)
  
  Nmap done: 256 IP addresses (3 hosts up) scanned in 89.75seconds
  
  
  The above shown is the example of using nmap on a host this was carried out in terminal of my linux device and also it has detected the
  virtual system present mac addresses of the system are cencersored as this is only for educational purpose.So guys now practice this on
  your own systems and move a step ahead in this field i also suggest you to refer the cheat sheet for nmap as this is an these two phases
  are very important and always keep record of the information collected in these phases even a single vulnerable port can lead to a huge 
  impact on asset.
  
  tool link:- https://nmap.org/download.html (kali has it pre installed only windows users need to download).
 
 # [Red Hawk](https://github.com/Tuhinshubhra/RED_HAWK) 
 
 This tool is also one of the most powerful recon tool
  
 video tutorial :- Comming Soon
 
  

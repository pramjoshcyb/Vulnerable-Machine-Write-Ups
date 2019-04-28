# Drupal - Content Management System
## Method: **Metasploit**
## Student Name: **Pramath Joshi**
## Instructors: **Mr Sayasmito and Mr David Jorm**
## Institution: **Coder Academy Melbourne**
## Aim: To Escalate Privileges and Achieve ROOT Access
## Exploit Name: **Drupalgeddon**

# Background

- Drupal is a content management software and is used to   develop various websites and applications that users     use every day. The tools that are offered with Drupal    assist in making the website versatile and has           structured content that dynamic web experiences need. 

- It is also an excellent choice for creating combined digital frameworks by extending to thousands of          add-ons.

- The projects that are accomplished using the Drupal      software is open source, meaning that anyone can         download, use, work on and share with others.  

- It’s always free 
 
 # Methodology Step By Step:

 1. To establish what network, I am on in Kali Linux, I inserted a command called: ***ifconfig***

 ![Photo.png](./Images/Photo.png)

As you can see from the image, the output is telling me that my systems Internet Protocol (IP) Address that is assigned to me is 192.168.211.132 which is a private network meaning it is restricted to either home or work environments. 

I can also let you know that because of the netmask being 255.255.255.0 I immediately know that I am on the 192.168.211.0 network. The subnet mask being /24 lets me know that. 


2. To view what networks are available around my environment I issued a command called: ***netdiscover -r 192.168.211.0***


 ![netdiscovercommand.png](./Images/netdiscovercommand.png)

As you can see from the output, I can see 3 IP addresses and the vendors are all VMware’s. I can see that the IP 192.168.211.1 is my gateway address since it starts with a .1. 

I can see that 192.168.211.254 is the last usable address. I can finally see that the Drupal machine must be on 192.168.211.133 with the above MAC address which is the physical address.

3. 

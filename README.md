# Installing Pfsense on VM - Lab
<img src="https://img.shields.io/badge/-pfSense%20Firewall-blue?style=for-the-badge"></img>

## Objective
This lab includes steps for installing pfsense firewall in a VM for leanring and educational purpose .

### Skills Learned

- What is Pfsense
- Installing pfsesne on VM
- Setting up pfsense on VM.

### What is pfsense ?
PFSense is a software-based firewall solution. It's like a virtual wall that sits between your computer network and the outside world (the internet), controlling the flow of data in and out of your network.

Here's what it does in simple terms:

Security: It helps keep your network safe from unauthorized access and potential threats by filtering incoming and outgoing traffic.

Control: You can set rules and policies to determine what types of data can enter or leave your network. For example, you can block certain websites or restrict access to specific services.

Monitoring: It allows you to keep an eye on what's happening on your network, such as which devices are connected and what they're doing.

Customization: You can tailor the firewall settings to meet the specific needs of your network, whether it's for a home network or a large enterprise.

Overall, PFSense is like a digital bouncer for your network, keeping the good stuff in and the bad stuff out.

### Tools Used

- Pfsense CE edition Free
- Hypervisor either Vmware or Oracke Virtualbox
- 7Z file archiver Free

### Diagram Reference :
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/644a7e51-5b75-436a-8780-f51c92fa0249)


### Steps
### Step -1 Download Orcale Virutal box or Vmware 
<a href="https://www.virtualbox.org/wiki/Downloads">Oracle Virtual Box</a><br>
<a href="https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html.html">Vmware</a><br>
### Step -2
Download ISO image CE (Free) from pfsense Official website link below
https://www.pfsense.org/download/
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/b6b4a6f9-9294-4d73-bc95-8fabdd9afa20)

![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/7088607b-fb5e-417f-9f34-2dd67ce6a83d)

### Step -3
Download & install 7z free file archiver software
Link : https://www.7-zip.org/

### Step 4
Extract pfense downloaded file using 7z
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/3be46a3f-fd49-4deb-bac3-923705361cf0)

### Step 5
Create new virtual machine with these settings . Dont forget to give ISO image location the file you extracted 
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/c6d46b04-11bc-4add-8872-c36e2a4468f4)

<b> Allocate resources as per your system specs. I am allocating 4GB of RAM
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/c9acf40f-8251-4227-9134-2576eab2a347)

<b> Select min 10GB of harddisk space I have chosen 20GB if you need to intall more packages !</b>
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/702503f9-d29c-40bf-827c-d8b73c947faa)

Click Finish.

### Step 5
Setup Network Interfaces (WAN)
Adapter -1
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/63350c0c-d345-4607-a41b-e6076c9e2857)

Adapter-2 (LAN)
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/e4cb11d2-458b-4ba2-8871-2a545d483a8b)

Adapter-3 (DMZ)
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/55cb5c61-8298-4a2f-9372-54730400ea1b)

### Step 6 
Installing Pfsense
Seelct Virtualmachine & Click START
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/c91ef1f7-7ca4-4b03-ae72-fc1c5e15c7e2)

![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/8d1b96b3-4b3c-48d3-bcc6-564af42fe26b)

Press Accept :
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/df6a41f6-0294-412c-b4ed-283f07f488c7)

Press Enter  to install Pfsense:
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/22c5f164-26c1-4592-802d-246bf4b15af2)

Press Enter :
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/d6e665d5-916d-40df-a1a1-86e4f5f4fac3)

Press Enter:
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/b4cce404-d960-4d96-8833-a051af7645aa)

Press Enter : Installing on Single disk
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/2a14e71c-f95d-4ac3-8ad0-ae70734cab2a)

Pree Space Bar to seelct then Press Enter :
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/9a0c942e-c5b6-44fc-b454-31ee52c0c394)

Use Tab key to select YES then Press Enter :
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/cdb04ad5-43da-44e4-b6d8-f5471fee4d43)

Installtion will start will take time so be pateint!
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/3f72d511-c138-45f2-88e2-d5b11f34e44c)

Once installtion completed will see this screen
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/f8effe38-ca95-4bfe-9fc2-4c3e950b5242)

IMPORTANT : to remove ISO file we used fro installtion before REBOOT else process will start again !
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/4dd35067-aecb-4b84-9119-788539d974fc)

Click Force unmount option 
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/fcb34ede-6391-45c8-8fb2-a374635265ce)

Then Press Enter To REBOOT now !
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/1c83f11a-a49c-4580-8eb6-064762f32cca)

Type EXIT to reboot
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/c8d883c5-2870-41f4-a966-3bb2db4365a3)

Ignore the errors:
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/03002cad-212b-489a-9748-10c2a1b25a2d)

![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/1ca21704-124a-417f-a8ad-678fe9025c74)


![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/51f7d66f-1cb9-4f33-a5a5-f39b6f843c44)

### Step -7 After reboot Pfsense will automatically sense interfaces:
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/181fb213-7381-4ea8-8fad-be21cf378b19)

DHCP will be enabled as default on LAN interface , Adapter -1 as WAN identifed and other 2 interfaces as DMZ & LAN Default range is shown as well.
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/adae4355-da4a-4301-a0eb-80fc39124693)

### Step 8 Configure Pfsense
To configure Pfsense we need to install other VM you can use Windows Or Linux ISO for this you can search google for win 10 ISO or ubuntu (Pre built images) then downlaod ISO files and install to VM

After Ubuntu installation assign internal network from settings.
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/cdbffc6d-e6e4-4a10-9642-95f226d31235)

After assigning internal network run ifconfig or ip a from terminal to check if it picked up IP address from pfsense DHCP range like 192.168.XX if its then its setup correctly.
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/1a6660c7-c206-4fb2-857d-a9bde3db08fe)

Try ping the pfsense LAN interface on IP 192.168.1.1 if you see response then its connected & okay .
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/f448292f-f4ac-456c-835f-741bfef35ab0)

From Ubuntu machine Open browser and type in 192.168.1.1 pfsense WAN interface IP :
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/bf409b57-c7fb-46a2-ae2e-4c959726c002)

Click Acceept the Risk & Continue

![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/e9c77cfb-cd6d-4720-b1e0-e47ecda72efa)

You will see Pfsense login screen. Username admin & Password pfsenser ( all small)
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/54a40d7d-3476-4ec8-900f-0e88cde98a0e)

![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/2a4555e8-2b30-424e-9b0b-16878aba92b1)

Click NEXT and hurray you have successfully installed Pfsense on your VM .
![image](https://github.com/syedhnaqvi/pfsense/assets/39069507/83f07f42-08dd-4ec5-a3bf-00de05760f11)




  ## Links & References
- <a href="https://youtu.be/mWqYyl89QaY](https://www.youtube.com/watch?v=LX-Y-99zJ3M)">Installing & Setting up Pfsense firewall</a>


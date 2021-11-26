SYNOPSIS


Just like any Kali-linux application installed in a virtualbox, we will be using it for pentestiong purposes. Try conducting an internet search for the phrase “pen testing tools.” You’ll find that many of the resources include Kali in their “best of” lists. Kali is immensely popular with both pen testers and hackers. The reason for the cross-cultural appeal is that the tools included in Kali can be used for beneficial or malicious purposes.One of the biggest reasons cyber professionals use and often prefer Kali Linux is the fact that all of the  original source code is open source, meaning that the system can be tweaked to the liking of the cybersecurity professional that is using it.  Which this is not necessarily done often, it does provide the option to personalize Kali for specific cybersecurity tasks. Kali Linux also comes with multi language support.

PROBLEMS IT SOLVES:


With Kali Linux, pentesters are able to test for vulnerable systems so they can patch them. It helps companies or organizations to identify holes in thier systems and to avoid unethical activities, they engage pentesters who use this tool (Kali) to help solve their problems.


Installing Kali-Linux on DigitalOcean

DigitalOcean is a cloud computing vendor that provides an infrastructure as a service (Iaas) platform for developers. Like Amazon Web Services(AWS), Google and Microsoft Azure DigitalOcean competes with these web services that allows scale by deploying DigitalOcean applications that run parallel across multiple cloud servers without compromising performance.

In this project, we attempt to install Kali-Linux on this plaform and use it to hack a windows systen on our network.


Installing Process


![3](https://user-images.githubusercontent.com/64130406/143523567-bce73234-0415-4150-a834-c72501c107e5.JPG)
This image shows the upload in progress.


![4](https://user-images.githubusercontent.com/64130406/143523678-452a54f3-f7f9-4dea-ae4b-4700e2678a46.JPG)
After a long wait, the upload came up as an error. 


![1](https://user-images.githubusercontent.com/64130406/143523086-0d36853e-93ee-4d54-9515-9a96169e5846.JPG)
We got this error code when we decided to upload the kali .iso file on Digital Ocean. Digital Ocean only accept files with these extensions 

*.gz 
*.bz 
*.bz2 
*.vmdk 
*.vhdx 
*.qcow 
*.qow2 
*.vdi 
*.raw 
*.img 
*.xz.

![2](https://user-images.githubusercontent.com/64130406/143523252-7fcc53e0-fe59-4889-8c45-a8571d877a41.JPG)
We decided to upload Kali-Linux-2021.2-virtualbox-amd64-disk001 which we had on our VirtualBox and had the .vdi extension. We had a warning that the file size was 39GB and it is very close to most browser limits, we still went ahead with the upload. 

Most Old versions of Kali works fine and so if 2020 or 2021 doesn't work as we couldn't get a GUI, try the 2019 and following the process below, convert it into a vmdk file and upload. With 2019, you get a Live am64 where you can run a GUI.

![5](https://user-images.githubusercontent.com/64130406/143523964-e8f4341a-cad9-4bce-8665-a7cce00748a9.png)
Open Command promt and run as administrator


![6](https://user-images.githubusercontent.com/64130406/143524029-cf4ab5e9-43b8-4e6e-bafa-2b2033642f37.JPG)
On the command line, enter cd "C:\Program Files\Oracle\VirtualBox" to change the directory to the Oracle VirtualBox. 


![7](https://user-images.githubusercontent.com/64130406/143524070-cf5dbbe1-5742-4a68-aa8f-49abf9ec7f95.JPG)
We used the convertfromraw --format command to covert the .iso to .vmdk

VBoxManage convertfromraw --format VMDK "G:\Cyber Security and Networking Classes\kali-linux-2019.1b-installer-amd64.iso" "G:\Cyber Security and Networking Classes\kali-linux-2019.1b-installer-amd64.vmdk"


![8](https://user-images.githubusercontent.com/64130406/143524502-5a22757e-fac1-4982-8d72-451af663edec.JPG)
Locate the .vmdk. 

v Uploading the .vmdk file to Digital Ocean.

![9](https://user-images.githubusercontent.com/64130406/143524599-6be6f7a5-7df9-41d9-8562-18af06e41d34.JPG)
Open Digital Ocean, on the right side locate the Manage tab. 


![10](https://user-images.githubusercontent.com/64130406/143524667-342f1c26-4c4d-4b69-b780-f6235da2dbd6.JPG)
We clicked on the Images and locate the .vmdk file, we can also drag and drop the .vmdk file 


![Capture](https://user-images.githubusercontent.com/64130406/143524855-c5b53a43-17ee-4bb8-92d4-c63e7c1089fb.PNG)
Now our .vmdk file is uploaded successfully on Digital Ocean. 





REFERENCES
You cam refer to the following links for additional references.
1. https://www.kali.org/blog/kali-linux-in-the-digitalocean-cloud/
2. https://www.how2shout.com/how-to/how-to-convert-iso-to-vdmk-or-vdi-using-virtualbox.html


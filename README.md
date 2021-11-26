Installing Kali-Linux on DigitalOcean

DigitalOcean is a cloud computing vendor that provides an infrastructure as a service (Iaas) platform for developers. Like Amazon Web Services(AWS), Google and Microsoft Azure DigitalOcean competes with these web services that allows scale by deploying DigitalOcean applications that run parallel across multiple cloud servers without compromising performance.

In this project, we attempt to install Kali-Linux on this plaform and use it to hack a windows systen on our network.


Installing Process


![3](https://user-images.githubusercontent.com/64130406/143523567-bce73234-0415-4150-a834-c72501c107e5.JPG)
This image shows the upload in progress.


![4](https://user-images.githubusercontent.com/64130406/143523678-452a54f3-f7f9-4dea-ae4b-4700e2678a46.JPG)
After a long wait, the upload came up as an error. 


![1](https://user-images.githubusercontent.com/64130406/143523086-0d36853e-93ee-4d54-9515-9a96169e5846.JPG)
We got this error code when we decided to upload the kali .iso file on Digital Ocean. Digital Ocean only accept files with the extensions 

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



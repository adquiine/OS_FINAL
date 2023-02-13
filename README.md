# OS_FINAL
There are all the explanations for final exam
#	Full Name,	Group 
1)	Mukhamedzhan Gabituly	CS-2122
2)	Elnur Khamzin	CS-2122
3)	Nazerke Adilgali	CS-2122

Task 1:


Screenshots of the code compilation result:


![image](https://user-images.githubusercontent.com/86833038/218450877-09f11949-274a-497e-bf14-cf78429a11f2.png)



Task 2:
Screenshots of the code compilation result:
Direct IP Connection:
Assign a public IP address directly to the virtual machine.
For example, we will choose google.com domain (ip - 142.250.180.110)
This approach necessitates the virtual machine to possess its own publicly accessible IP address, which may not always be attainable since public IP addresses are a scarce resource.
The virtual machine can then access the Internet directly.
So, we can verify it using ping command by sending our traffic packets to this public ip.


<img width="488" alt="image" src="https://user-images.githubusercontent.com/86833038/218451066-5170f6b1-2c79-4906-b7b0-157daee2d528.png">


NAT Connection:
The virtual machine is assigned a private IP address, and a NAT gateway is used to translate the private IP address to a public IP address.
This allows the virtual machine to access the Internet while preserving the limited number of public IP addresses.
NAT is commonly used in home networks and virtual private clouds.
And we can also verify the network to check internet connection on our OS with NAT by using ping command:
Every our packets were sent successfully!


Proxy Server Connection:
A proxy server acts as an intermediary between the virtual machine and the Internet.
The virtual machine sends its Internet requests to the proxy server, which then makes the requests on behalf of the virtual machine.
The proxy server may provide additional security and ﬁltering features, such as blocking certain types of Internet traffic.
Here, we used curl command to see website moodle.astanait.edu.kz with proxychain that changes our real ip address in proxy server and send with another IP address.



Task 3:
Screenshots of the code compilation result:

To create a simple kernel module in Kali Linux
First, install the necessary packages for kernel module development

<img width="479" alt="image" src="https://user-images.githubusercontent.com/86833038/218451382-10dc2453-617d-459f-ba52-c4af0a91c1d8.png">


Then we created .c ﬁle to execute our code to add our kernel module!


![image](https://user-images.githubusercontent.com/86833038/218451402-47bcb0dd-dd47-45a0-81ba-6ab53b43eb46.png)


The correct path to the Linux kernel headers should be speciﬁed in the Makeﬁle to build process for your kernel module without any error!
Then loaded the module into the kernel. And wee can verify that the module has been loaded by using lsmod | grep my_module and it shows us ourmodule.
Here proof about adding our module to kernel. I removed it, then when show it again here already no my_module kernel module.

![image](https://user-images.githubusercontent.com/86833038/218451450-2d20f1f6-30d8-426f-a863-3096643d4877.png)

<img width="296" alt="image" src="https://user-images.githubusercontent.com/86833038/218451502-cbfc6b4a-340e-49e6-8482-19923b4ba888.png">


Creating a kernel module has several advantages, including:
Increased performance, better resource utilization, improved system functionality, improved security and so on.


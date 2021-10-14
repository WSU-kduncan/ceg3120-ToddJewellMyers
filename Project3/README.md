# CEG 3120 - Project 3


## Part 1 

# VPC
* VPC (Virtual Private Cloud) is dedicated virtual network that allows us to use the services of the server from AWS over the internet the one we are currently making is considered a Public Cloud. its purpose to is make a digital connection over a network using a virtual network to allow us to use its services from anywhere which gives us the ability to access data anywhere.

## image
![screenshot](images\VPC2.png)

# Subnet

* The Subnet is a range of IP addresses in you VPC used to allow computers to talk directly to one another without a gateway. 

## image
![screenshot](Subnet2.png)

# Gateway 

* A gateway is a node (router) in a network this is a important stopping point for the data on its way to or on its way from other networks.
because of this we can send our data back and forth being able to communicate with one another. 

## image
![screenshot](Gateway.png)

# Route Table

* Routes are used to direct where your network traffic will go. This will be used with our cloud to direct traffic within the network where you want it to go and send out data out into the world.

## image
![screenshot](routetable.png)

# Security Group 

* Security Groups work outside and inside the VPC the rules allow you to filter the traffic using protocols and port numbers. This will be our firewall for the network 

## image
![screenshot](SecurityGRoups.png)

## Part 2

* when choosing an AMI I chose the Ubuntu Server 20.04 LTS (HVM), SSD Volume Type - ami-09e67e426f25ce0d7 (64-bit x86) / ami-00d1ab6b335f217cf (64-bit Arm) i chose the instance that was free the t2.micro with 1 cpu and 1 GB of memory. I called the instance Myers-instance 

* I connected it when setting up the instance, it asked for it i made sure to delete the preconnected one and typed in the Myers-VPC.

* I want to reserve the eleastic IP so that amazon doesnt ask for the IP back if someone was to purchase the IP I was using this would mean i would have to go back and correct things which I would prefer not to when able.

* The volume was attached when we created the EIP for the instance 

* To tag the instance you need to go to the Tags table and click the Manage tags tab from there you can add the name you wish for it to be.

* The Security group was added when creatign the instance and was added once it was done and created.

* I reserved the EIP I associated the instance and myers-eip by clicking on the actions tab next to the allocate Elastic IP address click associate tab then type in your instance with the instanbce field 

## image
![screenshot](instance.png)

* changing the hostname to Myers-Ubuntu
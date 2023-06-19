---
title: "Cloud Computing Service model"
datePublished: Mon Jun 19 2023 17:55:14 GMT+0000 (Coordinated Universal Time)
cuid: clj35pvef000f09jpg3vzh39w
slug: cloud-computing-service-model
tags: cloud, azure, saas, cloud-computing, sajjadrahman

---

Now let's dive into IaaS , PaaS and SaaS

Infrastructure as a Service ( IaaS)

Platform as a Service ( PaaS)

Software as a Service ( SaaS ) 

Identify appropriate use case for each cloud service ( IaaS , PaaS and SaaS )

## **Infrastructure as a Service ( IaaS)**

1. Delivers compute infrastructure, typically a platform visualization environment as a service.
    
2. Cloud providers build data centers, managing power, scale , hardware, networking , storage, distributed system, etc 
    
3. Rather than purchasing servers, software, data center, space, or network equipment, clients instead buy those resources as a fully outsourced service. 
    

Example: AWS EC2, Azure VM, and GCP Compute Engine 

## **Platform as a Service ( PaaS)**

Providers environment for building, testing , and deploying software applications; without focusing on managing the underlying infrastructure 

1. Its an offering that provides platform for developing running and managing applications worrying about infrastructure provisioning and maintenance 
    
2. Cloud providers offer an Internet-based platform to developers who create services.
    

**Examples :** 

* AWS Elastic Beanstalk 
    
* Azure App Service
    
* Google App Engine
    

## **Software as a service ( SaaS )**

* SaaS is a software delivery methodology that provides licensed multi-tenant access to software and its function remotely as a web-based service 
    
* From the end user’s point of view apps are located in the cloud and it is almost always accessible through a web browser 
    
* Any application hosted on a remote server that can be accessed over the internet is considered as SaaS 
    
* Usually billed based on usage and a multi-tenant environment   
    

![](https://lh6.googleusercontent.com/lalm-U_rZcw2SRotMvzV6GFyC5UNxzQCfwlqV-tZAAUIr6wge_l_rPHWYeyENwvPfiPBn-hUiMPmimgggeouIECrq3xHhItUCHHVT3P0LpXNqG1LuTfmSOCjCPljt6k371ZZSWZBqASZuEyzbbCCAPI align="center")

### **Disadvantages of Public cloud** 

1. Decent Internet Connectivity is mandatory
    
2. Can be costly if resources are no managed properly
    
3. Restricted or limited control of Infrastructure 
    
4. Risk of vendor lock in 
    
5. Data security and privacy concerns   
    

![Cloud Service Models](https://lh6.googleusercontent.com/hCLC_JBEl2LqMaiWbDjn1DNWAib_3GYaY-W0uJo9hTGeURJ20pYl2v3ahQSquWUBL1jxgeUnFgWKT41iikGcAVVbvR2ONWj7pUkCXyhqz92mlglDGSNqZd3ppWbV9dDRmG-xSsZecsuRqGCHzqByPtw align="center")

## **Azure Architectural  component** 

#### **Regions**

* Regions are made up of one or more data centers in the close proximity 
    
* Provide flexibility and scale to reduce customer latency 
    
* Preserve data residency with a comprehensive compliance offering 
    

**What are the benefits of so many azure regions ?**

I call a request and the response time is long due to being far away from the data center or region . It not user friendly 

`One regions has 3 availability zones` 

More regions need consumer request calls . It made to reduce the latency of the customer  . If it is not built what happens the problem might be Request time is long and consumer feel boring and deprive from the services 

### **Availability zones**

1. Provide protection against downtime due to datacenter failure 
    
2. Physically separate data centers within the same region 
    
3. Ecah datacenter is equipped with independent power cooling and networking . If one is down other zones are available . Physically separated but strong;y connected 
    
4. Connected through private fiber-optic networks 
    

Means one file save automatically in three zones .  !;35 minutes 

[![](https://lh6.googleusercontent.com/k4GzrQ7O8Gv2ulz652A2pp5r-9xq581kHtpmTwjalSCd5Q3MdU-fMDoK-iwj7-t3frqwIBfOJDMwDyvsDmpw9HIIPpbERV9HsLT9W1bptbEat4eods7jzfF_wKuinDpapepZfzLeHEicdFitzSX8s_I align="center")](https://www.unixarena.com/)

Avoid downtime ( lost the data center ) split the datacenter in different place within the same region . 

### **Region Pairs** 

* At least 300 miles of separation between region pairs 
    
* Automatic replication for same services 
    
* Prioritized region recovery in the event of outage 
    
* Updates are rollout sequentially to minimize downtime 
    

`So why pairs in need ?` 

Ok , at first 3 files are saved in the region and 3 other files in the 2nd region . Do this for high availability . If the entire region is Down , there is hope to find the resources from to the second location means pairs location . 

`Data center are available in Availability Zones , Availability Zones are available  in the the Region . And Regions are available in the Geographics` 

## **Azure resources** 

Everything in the cloud is services .

Azure resources are components like storage , virtual machines , and networks that are available to build cloud solutions 

Virtual networks connected to the resources ( virtual machine ) are also resources .

![](https://lh3.googleusercontent.com/57A0lSLUESyjr19Nx9rHMiE8Aox_iDk2sXg1KFMagl0aSDpGFtroY0WxmEg42AT_e7LQAvSzTVtwUnCGdAE4Myw40P_d1Aq6nsFS2jqPLURevKuTFB4L-a4Yhzr58OtLRbqxRbbMPrnfL6zf6lho8PU align="center")

## **Resources Group** 

A resources group is a container to manage and aggregate resources in a single unit .

1. Resources can exist in different regions 
    
2. Resources can exist in only one group 
    
3. Resources can be moved to different resources groups 
    
4. Applications can utilize multiple resource groups 
    

Different resources group means that when I create a VM I select the region that is in central India . Ok fine now I  want to create storage resources , I select the region is Germany . Is it possible in two different places, yes . It is possible . 

Resources group is Logical Datacenter not physical 

For exam : resources and resource group   not necessary must be in the same region they can be different region 

## **Azure Subscription** 

`Subscription is billing boundary` 

An azure subscription provides you with authenticated and authorized access to Azure accounts

**Billing Boundary :** Generate separate billing reports and invoices for each subscription 

Access Control Boundary: Manage and control access to the resources that users can provision with specific subscriptions 

## **Management Group**

1. Management groups can include multiple azure subscriptions 
    
2. Subscriptions inherit conditions applied to the management group 
    
3. 10,000 management groups can be supported in a single directory
    
4. A management group tree can support up to six levels of depth .
    

Management groups can be nested means A management group inside has another management group , it can manage another group otherwise subscription can not be inside subscription   . a resource group like a subscription group . Remember one thing that Resources group are INDEPENDENT 

Thats all for the time being .
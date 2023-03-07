---
title: "Computer Networking"
seoTitle: "Computer Networking  and IPv4"
seoDescription: "Computer networks work layer by layer. Not fully complete at a time. The famous layer approach model is OSI MODEL."
datePublished: Tue Dec 13 2022 18:03:21 GMT+0000 (Coordinated Universal Time)
cuid: clcjcd8zz000008l3d27scu7z
slug: computer-networking
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670768253484/Ym6SWqby2.jpeg
tags: networking, computernetwork, wemakedevs

---

Whenever the terms Networking we show, we think it is computer networking. Simply to say networking means establishing connections.

### Flesh back of Data Communication

When we need to establish a connection there need very fundamental 5 components : \[ **Sender, Medium, Receiver, user, Message** \]

### Network Criteria

A certain number of criteria must be met by a network among them these 3 ( **performance, reliability, and security** ) are very important.

`Performance:` It can be measured in many ways where transit and response time are topmost. Transit time is the amount of time needed for a message to travel from one device to another. Where response times are between an inquiry and a response. Also, other factors are the number of users, transmission medium, and so on.

`Reliability:` It means the stability of the networks and is measured by the number of failure frequencies or the times take to recover.

`Security:` By names, we assume that data protected from

## The Internet Today

The Internet has come a long way since the 1960s. And it is not a simple hierarchical structure. It is made up of many wide- and local-area networks joined by connecting devices and switching stations. Today most end users who want an Internet connection use the services of Internet service providers (lSPs).

### Protocol

A protocol is a set of rules that govern data communication; the key elements of a protocol are syntax, semantics, and timing.

### Standards

Standards are necessary to ensure that products from different manufacturers can work together as expected.

## Network Model

Computer networks work layer by layer. Not fully complete at a time. The famous layer approach model is `OSI MODEL` . The layered approach is called peer to peer process.

The OSI MODEL in one picture.

[![OSI MODEL](https://cdn.hashnode.com/res/hashnode/image/upload/v1670949987323/7yHQCGNtd.png align="center")](https://www.bing.com/images/search?view=detailV2&ccid=L%2fMxY4bY&id=C37CE8E562F995A70267626DBB54E62B45235DE0&thid=OIP.L_MxY4bY2XddyY9QfS4SHAHaE6&mediaurl=https%3a%2f%2fi1.wp.com%2fsemiengineering.com%2fwp-content%2fuploads%2f2014%2f09%2fosi1.png%3fresize%3d930%252C617&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.2ff3316386d8d9775dc98f507d2e121c%3frik%3d4F0jRSvmVLttYg%26pid%3dImgRaw%26r%3d0&exph=617&expw=930&q=OSI+MODEL&simid=607997550944070185&FORM=IRPRST&ck=DFA8007EA6BD8D1E51582B8F0C21CD3A&selectedIndex=9&ajaxhist=0&ajaxserp=0)

Another model is called the TCP model. The difference between TCP and OSI is in TCP is divided into 4 parts whereas OSI is 7. The working procedure is almost the same.

## Logical Addressing

In computer networks, Addressing is one of the controversial topics. Unfortunately, we all are connected to this term.

Our devices either phones or PC, all have IP addresses. Now we are using `IPv4`

## IPv4 Address

An IPv4 address uniquely and universally defines the connection of a device it is 32 bits. Unique means one device has only one IP address, there is no possibility that 2 online device has the same IP.

32 bits means it has the number of addresses is 2^32 \[ 4,294,967,296 (more than 4 billion). \]

### IP address notations

There are two ways to show an IPv4 address: binary notation and dotted-decimal notation.

`binary: 01110101 10010101 00011101 00000010`

`dotted-decimal: 117.148.19.28`

Also, IP address is divided into 2 ways Classful and Classless

### Class Full Address

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670954067683/lB9OukJWY.png align="center")

Already we know that 32 bits divide into 4 octets and each octet has 8 bits.

The blue colors denote the Network Id and the Yellow colors denote the host id. The host id is for the end user.

**Class A:** 1 network and 3 host id mean 2^24 addresses are possibly generated by class A. ( `possible address = 2 ^ no of host octet` )

### Classless Addressing

Classless Addressing there are no classes, but the addresses are still granted in blocks.

#WeMakeDevs
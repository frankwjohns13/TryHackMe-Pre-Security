# TryHackMe Pre-Security Notes

## Table of Contents
- [Introduction](#introduction)
- [Module 1 - Introduction to Cybersecurity](#module-1---introduction-to-cybersecurity)
  - [Room 1 - Offensive Security Intro](#room-1---offensive-security-intro)
  - [Room 2 - Defensive Security Intro](#room-2---defensive-security-intro)
  - [Room 3 - Careers in Cyber](#room-3---careers-in-cyber)
    - [Security Analyst](#security-analyst)
    - [Security Engineer](#security-engineer)
    - [Incident Responder](#incident-responder)
    - [Digital Forensics Examiner](#digital-forensics-examiner)
    - [Malware Analyst](#malware-analyst)
    - [Penetration Tester](#penetration-tester)
    - [Red Teamer](#red-teamer)
- [Module 2 - Computer Fundamentals](#module-2---computer-fundamentals)
  - [Room 1 - Inside a Computer System](#room-1---inside-a-computer-system)
  - [Room 2 - Computer Types](#room-2---computer-types)
  - [Room 3 - Client-Server Basics](#room-3---client-server-basics)
  - [Room 4 - Virtualization Basics](#room-4---virtualization-basics)
  - [Room 5 - Cloud Computing Fundamentals](#room-5---cloud-computing-fundamentals)
- [Module 3 - Operating Systems Basics](#module-3---operating-systems-basics)
  - [Room 1 - Operating Systems - Introduction](#room-1---operating-systems---introduction)
  - [Room 2 - Windows Basics](#room-2---windows-basics)
  - [Room 3 - Linux CLI Basics](#room-3---linux-cli-basics)
  - [Room 4 - Windows CLI Basics](#room-4---windows-cli-basics)
  - [Room 5 - Operating System Security](#room-5---operating-system-security)
- [Module 4 - Software Basics](#module-4---software-basics)
  - [Room 1 - Data Representation](#room-1---data-representation)
  - [Room 2 - Data Encoding](#room-2---data-encoding)
  - [Room 3 - Python - Simple Demo](#room-3---python---simple-demo)
  - [Room 4 - JavaScript - Simple Demo](#room-4---javascript---simple-demo)
  - [Room 5 - Database SQL Basics](#room-5---database-sql-basics)
- [Module 5 - Network Fundamentals](#module-5---network-fundamentals)
  - [Room 1 - What is Networking](#room-1---what-is-networking)
  - [Room 2 - Intro to LAN](#room-2---intro-to-lan)
  - [Room 3 - OSI Model](#room-3---osi-model)
  - [Room 4 - Packets and Frames](#room-4---packets-and-frames)
  - [Room 5 - Extending Your Network](#room-5---extending-your-network)
- [Module 6 - How The Web Works](#module-6---how-the-web-works)
  - [Room 1 - DNS in Detail](#room-1---dns-in-detail)
  - [Room 2 - HTTP in Detail](#room-2---http-in-detail)
  - [Room 3 - How Websites Work](#room-3---how-websites-work)
  - [Room 4 - Putting it all together](#room-4---putting-it-all-together)
- [Module 7 - Attacks and Defense](#module-7---attacks-and-defense)
  - [Room 1 - The CIA Triad](#room-1---the-cia-triad)
  - [Room 2 - Cryptography Concepts](#room-2---cryptography-concepts)
  - [Room 3 - Become a Hacker](#room-3---become-a-hacker)
  - [Room 4 - Become a Defender](#room-4---become-a-defender)


---

## Introduction
Welcome to my notes for the TryHackMe Pre-Security learning path. \
You can view my TryHackMe Badges here -> [Badges](https://tryhackme.com/p/WickedWizard?tab=badges)

## Module 1 - Introduction to Cybersecurity

### Room 1 - Offensive Security Intro
Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

**What is Offensive Security?** \
"It involves breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access." - THM

**Tool Used**
- **Gobuster** - Takes a list of potential page or directory names and tries accessing a website with each of them.
- **Flags**
  - -u to state website
  - -w to use a word list

### Room 2 - Defensive Security Intro
Introducing defensive security, where you will protect FakeBank from an ongoing attack. \

**Think like a Defender** \n
"Defensive security is the process of defending and securing devices and systems." \

**What does a defender do?**
- Detecting and investigating attacks, and responding before damage occurs.
- Detecting Suspicious Activity - Use the Event Management tool to detect a suspicious IP address.
- Identifying the Attack - Security Analyst Dashboard to find what page they are trying to access.
- Stop the Attack - Use a firewall rule to block the attackers IP address.

### Room 3 - Careers in Cyber

#### Security Analyst ####
"Security analysts construct security measures to protect the company from attacks. Analysts explore and evaluate company networks to uncover actionable data." - THM

**Responsibilities**
- Working with various stakeholders to analyse the cyber security throughout the company.
- Compile ongoing reports about the safety of networks, documenting security issues and measures taken in response.
- Develop security plans, incorporating research on new attack tools and trends, and measures needed across teams to maintain data security.

**Relevant Career Guides** (Official Links)
- [Becoming a Cyber Security Analyst](https://tryhackme.com/r/careers/cyber-security-analyst)
- [How to Become a Level 1 SOC Analyst](https://tryhackme.com/r/resources/blog/become-level-1-soc-analyst)
- [A Day in the Life of a SOC Analyst](https://tryhackme.com/r/resources/blog/interview-with-soc-analyst)
- [The Ultimate SOC L1 Analyst Interview Guide](https://tryhackme.com/r/resources/blog/soc-analyst-interview-guide)
- [From Student to SOC Analyst: Hayden’s Success Story](https://tryhackme.com/r/resources/blog/haydens-success-story)


#### Security Engineer ####
"Security engineers develop and implement security solutions."

**Responsibilities**
- Testing and screening security measures across software
- Monitor networks and reports to update systems and mitigate vulnerabilities
- Identify and implement systems needed for optimal security

**Relevant Career Guides** (Official Links)
- [Becoming a Security Engineer](https://tryhackme.com/r/careers/security-engineer)
- [How to Become a Security Engineer](https://tryhackme.com/r/resources/blog/become-security-engineer)
- [A Day in the Life of a Security Engineer](https://tryhackme.com/r/resources/blog/interview-with-security-engineer)
- [Preparing for a Security Engineering Interview](https://tryhackme.com/r/resources/blog/security-engineer-interview-guide)
- [Becoming a Security Engineer: Richárd’s Success Story](https://tryhackme.com/r/resources/blog/richard-success-story)

#### Incident Responder ####
Incident responders respond to security breaches. Incident response metrics include MTTD, MTTA, and MTTR - the meantime to detect, acknowledge, and recover (from attacks.) 

**Responsibilities**
- Developing and adopting a thorough, actionable incident response plan
- Maintaining strong security best practices and supporting incident response measures
- Post-incident reporting and preparation for future attacks, considering learnings and adaptations to take from incidents

#### Digital Forensics Examiner ####
"If you like to play detective, this might be the perfect job. If you are working as part of a law-enforcement department, you would be focused on collecting and analysing evidence to help solve crimes: charging the guilty and exonerating the innocent."

**Responsibilities**
- Collect digital evidence while observing legal procedures
- Analyse digital evidence to find answers related to the case
- Document your findings and report on the case

#### Malware Analyst ####
"A malware analyst's work involves analysing suspicious programs, discovering what they do and writing reports about their findings. A malware analyst is sometimes called a reverse-engineer as their core task revolves around converting compiled programs from machine language to readable code, usually in a low-level language."

**Responsibilities**
- Carry out static analysis of malicious programs, which entails reverse-engineering
- Conduct dynamic analysis of malware samples by observing their activities in a controlled environment
- Document and report all the findings

#### Penetration Tester ####
"You may see penetration testing referred to as pentesting and ethical hacking. A penetration tester's job role is to test the security of the systems and software within a company - this is achieved through attempts to uncover flaws and vulnerabilities through systemised hacking. Penetration testers exploit these vulnerabilities to evaluate the risk in each instance. The company can then take these insights to rectify issues to prevent a real-world cyberattack."

**Responsibilities**
- Conduct tests on computer systems, networks, and web-based applications
- Perform security assessments, audits, and analyse policies
- Evaluate and report on insights, recommending actions for attack prevention

**Relevant Career Guides** (Official Links)
- [Becoming a Penetration Tester](https://tryhackme.com/r/careers/penetration-tester)
- [How to Become a Penetration Tester](https://tryhackme.com/r/resources/blog/how-to-become-a-penetration-tester)
- [Preparing for a Junior Penetration Tester Interview](https://tryhackme.com/r/resources/blog/jr-pentester-interview-guide)
- [From IT Support to Pentester: Tom’s Success Story](https://tryhackme.com/r/resources/blog/tom-success-story)

#### Red Teamer ####
Red teamers share similarities to penetration testers, with a more targeted job role. 

**Responsibilities**
- Emulate the role of a threat actor to uncover exploitable vulnerabilities, maintain access and avoid detection
- Assess organisations' security controls, threat intelligence, and incident response procedures
- Evaluate and report on insights, with actionable data for companies to avoid real-world instances

**Relevant Career Guides** (Official Link)
- [Red Teaming: Job Roles, Salaries & Opportunities](https://tryhackme.com/r/resources/blog/red-teaming-jobs-salaries-opportunities)


## Module 2 - Computer Fundamentals

### Room 1 - Inside a Computer System
**Learning Objectives:**
- After completing this room, you will be able to recognize and understand the functions of various computing components.

**Inside a Computer System:**
- **Motherboard:** The skeleton and nerves
- **Random Access Memory (RAM):** Short-term memory
- **Power Supply Unit (PSU):** Heart and Lungs
- **Central Processing Unit (CPU):** The Brains
- **Graphical Processing Unit (GPU)** Visual Cortex
- **Hard Disk Drive (HDD) + Solid State Drive (SSD):** Long-term memory

**What happens when you press the Start Button**
- **Step 1: Press the Power Button**
  - A signal is sent to the PSU to allow power to flow
- **Step 2: Fireware satrts**
  - The central system called *Unified Extensible Firmware Interface (UEFI)* or the *Basic Input-Output System (BIOS)* come to life
- **Step 3: Power-On Self Test (POST)**
  - Tests if every required component is present, configured correctly, and functioning.
- **Step 4: Select Boot Device**
  - The system searches for the location of our bootup routine.
- **Step 5: Initiate Bootloader**
  - Initiates the "load routine" to start it.

This was just a quick overview of the internal parts and what happens when you press the power button on your computer. 

### Room 2 - Computer Types
**Learning Objectives**
- Upon completion of this room, you will be able to identify and distinguish between different types of computers you use directly, such as laptops and smartphones, and indirectly, such as servers, IoT devices, and embedded systems. You will also understand what makes each type suited to its purpose.

\
Four types of computers that often look similar but serve very different purposes.
- Portable everyday computing
- Sustained performance at a fixed location

<div>

  | **Computer Type**  | **Screen and Keyboard** | **Main Purpose**                                  |
  |--------------------|-------------------------|---------------------------------------------------|
  | Laptop             | Yes                     | Portable everyday computing.                      |
  | Desktop            | Yes                     | Sustained performance at a fixed location.        |
  | Workstation        | Yes                     | Precision and reliability for professional tasks. |
  | Server             | No                      | Providing services to many users over a network.  |

</div>


<div> 

  **Hideng in everyday objects:**
  | Type              | What it is                                                        | Examples                                                         |
  |-------------------|-------------------------------------------------------------------|------------------------------------------------------------------|
  | Smartphone        | Pocket-sized computer optimized for battery life and connectivity | iPhone, Android phone                                            |
  | Tablet            | Touch-first computer with larger screen                           | iPad, drawing tablet                                             |
  | IoT device        | Network-connected device with a single purpose                    | Thermostat, smart doorbell, fitness tracker                      |
  | Embedded computer | Computer built into another device                                | Coffee maker controller, automatic door sensor, lamp dimmer chip |

</div>

IoT vs Embedded: Both can be small and single-purpose. The difference is connectivity. IoT devices connect to a network to report data or receive commands. Embedded computers might not connect to anything; they do their job inside the machine, often for years without anyone knowing they exist.


### Room 3 - Client-Server Basics
**Learning Objectives**
- Understand the Client-Server model
- Understand the following concepts on a surface level:
   - Client
   - Server
   - Protocol
   - Port
   - DNS
   - Network

**Key Terms:**
- **Client:** The one making the request. (E.g., A web browser requesting a webpage)
- **Server:** The one the request is made to.
- **Protocol:** How requests are made.
  - Commands the client and server understand.
  - Request structure.
  - Syntax used.
  - Response to valid requests.
  - Response to invalid request.
- **Port:** Identify a specific service running on a system. 
- **Domain Name System (DNS):** Converts a human readable web address into an IP address (like a phonebook).
- **Scheme:** Tells us which protocol was used: HTTP or HTTPS.
- **Host:** Tells us the name of the host we request resources from.
- **Filename:** Indicates which file we requested from the host. In our request, this is "/", which actually translates to "index.html".
- **Address:** Displays the IP address where the website is hosted. In our example, we are hosting the website on the same device. That's why the address 127.0.0.1 is shown.
- **Status:** This field indicates whether the request was successful. In our example, we received a "200 OK" status, which means that the request was successful.

**Web Communication** \
Hypertext Transfer Protocol (Secure), abbreviated as HTTP(S), is a stateless client-server protocol used for the World Wide Web. This means that each request is processed independently, without the server retaining information about previous requests. 

**HTTP Commands** \
The Request for Comments (RFC) document lists nine core commands. 
- GET - Used to retrieve a resource from a web server.
- POST - Sends data to a server.
- PUT - Used to create or update a resource.
- DELETE - Instructs a server to remove a resource.
- PATCH - Used to apply partial modifications to a resource. 
- HEAD - Requests only the headers of a resource.
- OPTIONS - Used to request information about the communication options available.
- CONNECT - Special request type used to establish a tunnel through an HTTP proxy.
- TRACE - A diagnostic tool for instpecting the request chain between the client and server.

### Room 4 - Virtualization Basics
Have you ever considered how expensive and inefficient it would be if every piece of software or every website required its own physical server? 

**Virtualization was created to solve exactly this problem.** 

**Learning Objectives:**
- Understand why managing applications on individual physical servers is inefficient.
- Learn how virtualization addresses hardware utilization and scalability challenges.
- Understand the components of a lab machine.
- Learn how containers have further optimized hardware utilization for applications.

**One Application per Server**

If each application required its own server that would mean a company that wanted to run a website, have a database, an email service, and an internal app would need four seperate servers. This creates problems:
- **High cost:** Buying multiple physical servers is expensive, costs more in electricty, cooling, maintenance, and space.
- **Low utilizaiton:** Most applications don't use the full capacity of the server. So a lot of time is spent idle while waiting for a request.
- **Slow deployment:** Setting up physical servers takes days or weeks.
- **Hard to scale:** If an applicaiton needed more resources, you'd have to buy another physical server.

**What if multiple applications could be run on the same server safely?** 

**Enter virtualization:** A virtualization layer, called a hypervisor, was introduced to act as a referee between lab machines and allow each virtual computer to behave independently, like a physical computer.

Hypervisors have two main types of implementation, each of which is used for specific scenarios, from home labs to large data centers:
- **Type 1** hypervisors run directly on the physical hardware, making them fast, efficient, and ideal for servers and professional environments.
- **Type 2** hypervisors run within an existing operating system, making them easier to install and ideal for learning, testing, or small setups.

<div>

  | Use Case              | Type 1  | Type 2  |
  |-----------------------|---------|---------|
  | Test Malicious Files  |         |    X    |
  | Production Server     |    X    |         |
  | Database Server       |    X    |         |
  | Software Testing      |         |    X    |
  | Kali Linux            |         |    X    |
  | Data Center           |    X    |         |
  
</div>

**Lab Machines**\
Even though it’s virtual, it behaves as a real machine:
- It has its own virtual CPU, RAM, storage, and network.
- It can run any operating system (Windows, Linux, etc.).
- It’s completely isolated from other VMs. This means that if one VM breaks, the others continue to work.

**Containers**\
A container is a lightweight, isolated environment that runs a single application and all the necessary components to support it.

Containers behave like small, self-contained spaces because:
- They package the application and its dependencies (libraries, tools, versions).
- They share the host’s operating system, so they start almost instantly.
- They remain isolated from each other, so a misbehaving container doesn’t affect the others.
- They can run consistently on any machine, making them perfect for development, testing, and scalable deployments.


### Room 5 - Cloud Computing Fundamentals
If you created an application that you wanted a lot of people to use, you could host it on your own computer. However, you would have to share your IP address with everyone who wanted to access it. This can be difficult to remember — especially with long IPv6 addresses.

Additionally, your computer would need to stay online 24/7 for people to access the app at any time. What happens when your computer is turned off? What if more people try to access it than your network or hardware can handle?

These limitations make it very difficult for your app to scale and reach a large audience.

**That's when cloud computing comes to play and solves these problems!**

**Learning Objectives:**
- What is cloud computing
- Service models of cloud (IaaS, PaaS, SaaS)
- Cloud Types (Private/Public/Hybrid)
- Benefits of cloud computing
- How big companies are using the cloud

**Cloud Benefits and Characteristics:**
- **Scalability:** Easily scale up or down as your application's needs change.
- **On-demand self-service:** Create or remove servers and storage instantly, without waiting for hardware.
- **Pay only for what you use:** You are charged based on usage, not upfront costs.
- **Security:** Cloud providers protect the infrastructure with strong security measures.
- **High availability:** Applications keep running even if part of the system fails.
- **Global access:** Your application can be accessed by users anywhere in the world.

**Types of Cloud:**
- **Public Cloud:** Used by startups, websites, and global apps because it is affordable, easy to scale, and requires no infrastructure management. Public cloud services are preferable for nearly every use case.
- **Private Cloud:** Used by banks, healthcare, and government organizations because it offers greater control, customization, and compliance for sensitive data.
- **Hybrid Cloud:** Used by companies like e-commerce platforms that need to keep sensitive data private while still scaling publicly during high demand.

**Cloud Service Models:**
- **Infrastructure as a Service (IaaS):** You rent basic computing resources such as virtual servers, storage, and networking. You are responsible for managing the operating system and your application, while the provider manages the physical hardware.
- **Platform as a Service (PaaS):** The cloud provider manages the infrastructure and the operating system. You focus on building, deploying, and running your application without worrying about servers.
- **Software as a Service (SaaS):** You use a complete application over the internet. The provider manages everything, and you access the software through a browser or app, for example, Gmail or Zoom.

**Major Cloud Vendors:**
- **Microsoft Azure:** A strong competitor, especially in enterprise and hybrid cloud environments.
- **Amazon Web Services (AWS):** A pay-as-you-go basis, covering computing, storage, networking, databases, analytics, and machine learning. 
- **Google Cloud Platform (GCP):** Known for powerful data analytics, AI, and machine learning tools.
- **Alibaba Cloud:** A major player in Asia, offering competitive cloud services globally.
- **IBM Cloud:** Focuses on hybrid cloud and AI-driven solutions for businesses.
- **Oracle Cloud:** Focuses on enterprise applications and databases.


## Module 3 - Operating Systems Basics

### Room 1 - Operating Systems - Introduction
**Learning Objectives:**
- Understand what an operating system is and the role it plays
- Explain the core duties of an operating system
- Identify common OS types and their typical use cases
- Practice interacting with an OS to gather system information

**Key Terminology:**
- Operating system (OS)
- Kernel space
- User space
- Graphical user interface (GUI)
- Command-line interface (CLI)

#### **Operating System** 
The core software the coordinates everthing happening on a computer. It is the middle man between the hardware and the applications we use.

<div align="center">
  
  | User             |
  |------------------|
  | Applicaitons     |
  | Operating System |
  | Hardware         |

</div>

 Without an OS, each application would need direct control over the CPU, memory, files, devices, and security. This separation is intentional and helps prevent conflicts and security issues.
 - **Kernel space:** The privileged, locked-down core of the OS. It has unrestricted access to the hardware.
 - **User space:** Where all standard applicaitons run.

#### **Operating System Duties**
Every OS is responsible for a few core duties that allow your computer to run safely, efficiently, and predictably.

<div> 
  | **OS Responsibility**  | **What the OS Does**                                                               | **Example**                                                                |
  |------------------------|------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
  | Process Management     | Creates, schedules, prioritizes, and terminates programs.                          | Opening multiple apps, like your browser, music player, and social media.  |
  | Memory Management      | Allocates RAM to processes, protects the app's memory.                             | Allocates RAM to each open app keeping them isolated.                      |
  | File System Management | Organizes files into directories, handles naming, paths, permissions, and metadata | Creating new folders, saving photos, or setting a file to read only.       |
  | User Management        | Handles multiple user accounts, authentication, and permissions.                   | Logging in with your user name and password.                               |
  | Device Management      | Loads drivers and provides universal interface.                                    | Plugging in a new mouse, printer, or external hard drive.                  |

</div>

#### Operating System Security
At a basic level, your operating system handles:
- **Authentication:** Verifies who you are through login passwords and biometrics
- **Permissions:** Controls exactly what each user and app is allowed to read, write, or execute
- **Isolation:** Keeps every process in its own protected box (kernel/user space separation)
- **System Protection:** Safeguards critical system files and settings from unauthorized changes

**Graphical User Interface:** It provides the visual representation of all the information you want to access.
**Command Line Interface:** Text-based interface that allows you to enter commands to retrieve or manipulate information.

<div>
  
  | **OS Type** | **Primary Use Case** | **Key Characteristics** |
  |-------------|--------------------------------                           |--------------------------|
  | Desktop     | Personal computers, daily work, gaming, content creation. | Rich graphical interface |
  | Server      | Web hosting, databases, cloud services, back-end | Headless (no GUI), maximum uptime, multi-user, remote access |
  | Moblie      | Smartphones and tablets                          | Touch-based UI, power efficient, always connected, app sandboxing |
  | Embedded    | Appliances, cars, IoT devices,...                | Tiny footprint, runs on limited hardware |
  | Virtual/Cloud | Lab machines, containers, cloud instances | Lightweight, scalable, rapid deployment|
  
</div>

#### Real World Operating Systems
**Desktop**
- **Windows:** The most widely used operating system on personal computers Windows 10 (end-of-life), Windows 11
- **macOS:** Apple's desktop OS, known for its polished GUI and integration with other Apple devices Sonoma (14), Sequoia (15), Tahoe (26)
- **Linux:** Not a single OS but a family of open-source operating systems called distributions - Ubuntu, Debian, Fedora

**Server**
- **Windows:** Used in large networks, data centers, and corporate environments Server 2016, 2019, 2022, 2025
- **Linux:** The vast majority of web servers, trusted for its reliability and open-source nature Ubuntu Server, Debian, CentOS, Red Hat
- **Unix:** Large enterprises, finance, telecom, government IBM AIX, Oracle Solaris
  
**Mobile**
- **Android:** The most widely used mobile OS, which runs on phones, tablets, and smart devices Android 14 - 16, Manufacturer versions
- **iOS:** Apple's mobile OS running on iPhones, iPads, and other devices iOS 17, 18, 26

**Embedded and IoT Devices**
- **Embedded Linux:* Specialized OS built into devices with dedicated functions OpenWrt, Ubuntu Core, Yocto Project
- **Real-Time OS:** Designed for apps where tasks need guaranteed response times (aircraft controls)FreeRTOS, VxWorks, QNX

**Virtual and Cloud**
- **Cloud/VM:* Massive data centers that host websites, apps, and streaming services Ubuntu LTS, Amazon Linux, Rocky Linux
- **Container-optimized:** Lightweight alternatives to VMs that package just the app and its dependencies Alpine Linux, Bottlerocket AWS, Flatcar Linux

**Further Learning** (Official Links)
- [Windows Basics](https://tryhackme.com/room/windowsbasics)
- [Linux CLI Basics](https://tryhackme.com/room/linuxclibasics)
- [Windows CLI Basics](https://tryhackme.com/room/windowsclibasics)











### Room 2 - Windows Basics


### Room 3 - Linux CLI Basics


### Room 4 - Windows CLI Basics


### Room 5 - Operating System Security


## Module 4 - Software Basics


### Room 1 - Data Representation


### Room 2 - Data Encoding


### Room 3 - Python - Simple Demo


### Room 4 - JavaScript - Simple Demo


### Room 5 - Database SQL Basics


## Module 5 - Network Fundamentals


### Room 1 - What is Networking


### Room 2 - Intro to LAN


### Room 3 - OSI Model


### Room 4 - Packets and Frames


### Room 5 - Extending Your Network


## Module 6 - How The Web Works


### Room 1 - DNS in Detail


### Room 2 - HTTP in Detail


### Room 3 - How Websites Work


### Room 4 - Putting it all together


## Module 7 - Attacks and Defense


### Room 1 - The CIA Triad


### Room 2 - Cryptography Concepts


### Room 3 - Become a Hacker


### Room 4 - Become a Defender




---


<!-- End of File -->




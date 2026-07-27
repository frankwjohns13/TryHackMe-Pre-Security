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

**What is Offensive Security?** 
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
**Learning Objectives**
- Recognize the main hardware components of a computer and understand what each one does.
- Know the high-level sequence of events that occurs when you press the power button.

**Core Components (with simple analogies)**

<div>
  
  | **Component** | **Role** | **Analogy** |
  |------------------------|-----------------------------------------------------|--------------------|
  | Motherboard            | Central circuit board that everything else plugs into and communicates through | Skeleton + nervous system |
  | CPU (Central Processing Unit) | Executes instructions / does the actual computing | Brain |
  | RAM (Random Access Memory) | Fast, temporary working memory. Data disappears when power is cut | Short-term memory |
  | GPU (Graphics Processing Unit) | Handles graphics and parallel workloads (games, video, some AI) | Visual cortex |
  | Storage (HDD or SSD) | Permanent storage that keeps data even when the computer is off | Long-term memory |
  |PSU (Power Supply Unit) | Converts wall power into the voltages the components need and delivers it | Heart + lungs |
    
</div>

**Quick distinctions worth remembering**
- **RAM** is volatile (needs power). Storage is non-volatile.
- **HDD** = spinning magnetic disks (slower, cheaper per GB). SSD = flash memory (much faster, more expensive, no moving parts).
- Modern systems almost always use **UEFI** instead of the older **BIOS**, but people still say “BIOS” generically.

**What happens when you press the power button**
1. **Power button pressed:** Signal reaches the PSU → PSU starts supplying power to the motherboard and components.
2. **Firmware starts:** UEFI (or legacy BIOS) initializes. This is the very low-level software stored on a chip on the motherboard.
3. **POST (Power-On Self-Test):** Firmware checks that the essential hardware (CPU, RAM, etc.) is present and working. If something critical fails, you usually get beep codes or error messages.
4. **Boot device selection:** Firmware looks for a bootable device according to the boot order (SSD/HDD, USB, network, etc.).
5. **Bootloader is loaded and run:** The chosen device’s bootloader (e.g. GRUB, Windows Boot Manager) takes over and starts loading the operating system.

That’s the entire high-level sequence. Everything after step 5 is the OS taking control.

### Room 2 - Computer Types
**Learning Objectives**
- Identify and distinguish computers you interact with directly (laptops, phones, tablets) and indirectly (servers, IoT devices, embedded systems). Understand why each type is designed the way it is.

**Main Categories of Computers**

<div>

  | **Computer Type**  | **Screen and Keyboard** | **Main Purpose**                                  | **Key Design Focus** |
  |--------------------|-------------------------|---------------------------------------------------|---------------------------------------|
  | Laptop             | Yes                     | Portable everyday computing.                      | Battery life + mobility |
  | Desktop            | Yes                     | Sustained performance at a fixed location.        | Power, expandability, cooling |
  | Workstation        | Yes                     | Precision and reliability for professional tasks. | High stability, specialized hardware (CAD, video, science, etc.) |
  | Server             | No                      | Providing services to many users over a network.  | Reliability, uptime, remote management |

</div>


  **Computers Hidem in Everyday Objects:**
  
<div>   
  
  | Type              | What it is                                                        | Examples                                                         |
  |-------------------|-------------------------------------------------------------------|------------------------------------------------------------------|
  | Smartphone        | Pocket-sized computer optimized for battery life and connectivity | iPhone, Android phone                                            |
  | Tablet            | Touch-first computer with larger screen                           | iPad, drawing tablet                                             |
  | IoT device        | Network-connected device with a single purpose                    | Thermostat, smart doorbell, fitness tracker                      |
  | Embedded computer | Computer built into another device                                | Coffee maker controller, automatic door sensor, lamp dimmer chip |

</div>

**IoT vs Embedded - The Key Difference**
- **IoT** → has network connectivity (reports data or receives commands)
- **Embedded** → often has no network connection; it just does its job silently inside the device for years

### Room 3 - Client-Server Basics
**Learning Objectives**
Understand the client-server model at a surface level, including these concepts:\
Client · Server · Protocol · Port · DNS · Network

**Key Terms**
<div>
  
  | **Term** | **Simple Definition** |
  |----------|------------------------------------------------------------------------------|
  | Client   | The side that makes the request (e.g. your web browser asking for a webpage) |
  | Server   | The side that receives and responds to the request |
  | Protocol | The agreed set of rules for how the client and server talk to each other (commands, request format, responses for success/failure) |
  | Port     | A number that identifies a specific service running on a computer (e.g. web servers usually listen on port 80 or 443) |
  | DNA      | Domain Name System - converts a human-readable name (google.com) into an IP address (like a phone book) |
  | Network  | The connection that lets the client and server reach each other |
  
</div>

**Breaking Down a Web Request (example fields you’ll see)**

<div>

  | **Field**       | **Meaning** |
  |-----------------|-------------------------------------------------------------------------------------|
  | Scheme          | The protocol being used (*http* or *https)                                          |
  | Host            | The name of the server you’re talking to                                            |
  | Filename / Path | The specific resource requested (often / which maps to index.html)                  |
  | Address         | The IP address of the server (e.g. 127.0.0.1 when it’s running on your own machine) |
  | Status          | Result of the request (e.g. 200 OK = success)                                       |
  
</div>

**Web Communication – HTTP / HTTPS**
- **HTTP(S)** = Hypertext Transfer Protocol (Secure)
- Stateless client-server protocol used by the World Wide Web
- Stateless means every request is independent – the server does not remember previous requests by default

**Core HTTP Methods (Commands)**
<div>

  | **Method** | **Purpose**                                      |
  |------------|--------------------------------------------------|
  | GET        | Retrieve a resource                              |
  | POST       | Send data to the server                          |
  | PUT        | Create or completely replace a resource          |
  | DELETE     | Remove a resource                                |
  | PATCH      | Apply partial modifications to a resource        |
  | HEAD       | Get only the headers (no body)                   |
  | OPTIONS    | Ask what methods/options the server supports     |
  | CONNECT    | Establish a tunnel (usually through a proxy)     |
  | TRACE      | Diagnostic – show the request path (rarely used) |
  
</div>

### Room 4 - Virtualization Basics

**Learning Objectives**
- Understand why running one application per physical server is inefficient
- See how virtualization solves hardware utilization and scalability problems
- Know the basic components of a lab/virtual machine
- Understand how containers further improve efficiency

**The Old Problem: One Application per Physical Server**\
Running a website, database, email service, and internal app on four separate physical servers causes:
- High cost – hardware, electricity, cooling, space, maintenance
- Low utilization – most servers sit mostly idle
- Slow deployment – setting up physical machines takes days or weeks
- Hard to scale – needing more resources means buying more hardware

**Solution: Virtualization**\
A hypervisor sits between the physical hardware and the virtual machines. It acts as a referee so each VM can behave like an independent computer while sharing the same physical resources safely.

**Two Types of Hypervisors**
<div>

  | **Type**                | **Where it runs**                   | **Best for**                                       |
  |-------------------------|-------------------------------------|----------------------------------------------------|
  | **Type 1** (bare-metal) | Directly on the hardware            | Production servers, data centers, high performance |
  | **Type 2** (hosted)     | Inside an existing operating system | Learning, testing, home labs, small setups         |
   
</div>

**Typical use-case mapping**
<div>

  | **Use Case**         | **Type 1** | **Type 2** |
  |----------------------|------------|------------|
  | Test malicious files |    | ✓ |
  | Production server    | ✓ |    |
  | Database server      | ✓ |    |
  | Software testing     |    | ✓ |
  | Running Kali Linux   |    | ✓ |
  | Data center          | ✓ |    |
  
</div>

**Lab / Virtual Machines**\
Even though they are virtual, they behave like real computers:
- Have their own virtual CPU, RAM, storage, and network
- Can run any operating system (Windows, Linux, etc.)
- Are isolated from each other – if one breaks, the others keep running

**Containers**
A container is a lightweight, isolated environment that packages a single application + everything it needs (libraries, tools, versions).

**Key characteristics:**
- Shares the host operating system (much lighter than a full VM)
- Starts almost instantly
- Stays isolated from other containers
- Runs the same way on any machine → perfect for development, testing, and scaling

**Quick comparison**
- **VM** = full virtual computer (own OS)
- **Container** = just the application + its dependencies (shares the host OS)

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

**Learning Objectives:**
- Navigate the Windows graphical interface, including the desktop, taskbar, and Start menu
- Use File Explorer to browse folders, understand file paths, and organize files effectively
- Check system settings and personalize the Windows environment using the Settings app
- Use basic system tools like Task Manager and Windows Security to monitor performance and verify system protection

**Exploring the Windows Workspace**\
Before gaining access to the Windows Desktop, you must authenticate (prove your identity) to the system. The authentication process verifies your identity and determines the actions you're allowed to take once logged in.

**Typical Accounts:** 
- **Guest:** Restricted account for temporary access with minimal permissions.
- **Standard:** User account for everyday tasks. Cannot make system-wide changes.
- **Administrator:** Privileged account with full control over the system. 

Let's have a look at the Windows Desktop and cover some of its core features together. When you first log in, you're presented with two main areas.
- **Desktop:** The main workspace where files, folders, and shortcuts live
- **Taskbar:** A control strip that provides access to applications, system tools, settings, and notifications

**Core components and concepts**
1. **Desktop icons:** Shortcuts to items like the Recycle Bin, folders, and frequently used applications. It is fully customizable
2. **Start menu:** Primary way to access applications, settings, and power options. From here, you can log out, restart, or power off your machine
3. **Search:** Quickly find applications, files, folders, and system settings by using keywords
4. **Task View:** Allows you to see all currently open windows and quickly switch between them
5. **Pinned Applications and Folders:** Your most used applications and folders can be pinned here
6. **Network and Audio settings:** This section can be customized to suit your needs
7. **Date and Time:** Opens up to a full calendar. Date and time settings can be accessed here, too
8. **Notifications:** Displays computer or application notifications. Network and other settings can also be accessed

<!-- Image relating to the numbered terms above -->
<img width="520" height="457" alt="THM-Windows_Desktop" src="https://github.com/user-attachments/assets/5f5a2be9-18ad-44c6-9b8a-b040c358b11b" />

**Start Menu**
It is the area where we see what is available: apps, files, folders, settings, and power options.
<!-- Start Menu Image from TryHackMe's room -->
<img width="495" height="520" alt="THM-Windows-Start" src="https://github.com/user-attachments/assets/efd95624-b266-4411-86a9-4c7abc8f3349" />

*Image from the TryHackMe website found here:* [Windows Images](https://tryhackme.com/room/windowsbasics)

#### Updating Your Applications
Keeping your operating system and applications up to date is an important part of maintaining a secure and stable system

**Windows Updates**
Windows has a built in Windows Update tool. It can keep the OS and some native applications and security features up to date. 

**Updating Applications**\
Application updates work differently depending on how the software is installed.
- Built-in applications may update automatically in the background
- Third-party applications often include their own update mechanisms
- Some applications will prompt you to update upon launch
- Some require you to check for updates or download a new installer manually

#### Installing Applications
1. **Microsoft Store:** Provides a curated and safe option for installing apps to Windows, although it is not available by default on Windows Server
2. **From the Internet:** In many environments, apps are installed by downloading an installer directly from a trusted vendor's website. They usually come in an .exe or .msi file and guide the user through the installation process

#### Uninstalling Applications
In a Windows environment, there are multiple ways to uninstall programs. 
- Using the Microsoft Store for installed applications
- Add or remove programs feature in system settings
- Uninstall a program section of the Control Panel
- Using an application's built-in uninstaller

#### Diving Into Settings
There are two primary ways in which a Windows user can modify their environment. 
1. Windows Settings: A modern, centralized location for configuring system, device, personalization, and security settings in Windows
2. Control Panel: A legacy management interface that provides access to older system configuration tools still required for specific administrative tasks

#### The Task Manager
**Task Manager** is a built-in Windows tool that allows you to monitor what is happening on your system in real time.\
Task Manager has five tabs to help you keep track of your system.
1. **Processes:** Currently running apps and background processes, and their resource usage
2. **Performance:** Graphs and statistics for system resources such as CPU, memory, and network
3. **Users:** Currently logged-in users and used resources
4. **Details:** A more technical view of running processes, including process IDs (PIDs)
5. **Services:** Windows services and their current status (running or stopped)

#### Native Windows Security
**Windows Security**\
The **Windows Security** application is your central dashboard for managing Windows' built-in protection measures. It is divided into four main sections, each focusing on a different area of system security.
- **Virus & threat protection:** Helps detect and remove malicious software using real-time protection and customizable scans
- **Firewall & network protection:** Controls incoming and outgoing network traffic to help prevent unauthorized access
- **App & browser control:** Protects users from potentially unsafe apps, files, and websites
- **Device security:** Provides hardware-based protections that help secure the system

A closer look at the Virus & threat protection section of Windows Security on your workstation.
1. Open **Windows Security** using the shortcut in the *Show hidden icons* section of your taskbar. 
2. Select the Virus & Threat protection section.

#### Windows Defender Firewall
Windows Defender Firewall is a built-in firewall designed to help protect your computer from unauthorized network traffic.
- **Domain:** Used when a system is connected to an organization’s domain network
- **Private:** Intended for trusted networks, such as a home or lab environment
- **Public:** Used for untrusted networks, such as public Wi-Fi

Checking out the Advanced settings of Windows Defender Firewall, you can view
1. An overview of your firewall's inbound, outbound, and connection rules
2. A detailed view of each rule, including name, group, network profile, status, and action
3. Create new rules or filter your current view

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




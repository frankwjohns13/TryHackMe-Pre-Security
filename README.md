# TryHackMe Pre-Security Notes

## Introduction
Welcome to my notes for the TryHackMe Pre-Security learning path. \
You can view my TryHackMe Badges here -> [Badges](https://tryhackme.com/p/WickedWizard?tab=badges)

---

<details><summary><strong>Module 1 - Introduction to Cybersecurity</strong></summary>
  
## Module 1 - Introduction to Cybersecurity

<details><summary><strong>Room 1 - Offensive Security Intro</strong></summary>

### Room 1 - Offensive Security Intro
Hack your first website (legally in a safe environment) and experience an ethical hacker's job.

**What is Offensive Security?** 
"It involves breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access." - TryHackMe

**Tool Used**
- **Gobuster** - Takes a list of potential page or directory names and tries accessing a website with each of them.
  - -u → specify the target website
  - -w → specify the wordlist

**End of Room 1**

</details>

---

<details><summary><strong>Room 2 - Defensive Security Intro</strong></summary>
  
### Room 2 - Defensive Security Intro
**Goal:** Protect FakeBank from an ongoing attack.\

**What is Defensive Security?**\
“Defensive security is the process of defending and securing devices and systems.”

**What does a defender do?**\
- Detect and investigate attacks
- Respond before damage occurs

**Practical steps in the room:**
1. Detect Suspicious Activity → Use the Event Management tool to find a suspicious IP address
2. Identify the Attack → Use the Security Analyst Dashboard to see what page the attacker is trying to access
3. Stop the Attack → Create a firewall rule to block the attacker’s IP address

**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - Careers in Cyber</strong></summary>
  
### Room 3 - Careers in Cyber

  | **Role**                        | **Short Description**                                    |
  |---------------------------------|----------------------------------------------------------|
  | [Security Analyst](#security-analyst) | Builds security measures, analyzes networks, creates reports, and develops security plans |
  | [Security Engineer](#security-engineer) | Designs, tests, and implements security solutions; monitors and updates systems |
  | [Incident Responder](#incident-responder) | Handles security breaches; focuses on MTTD, MTTA, and MTTR metrics |
  | [Digital Forensics Examiner](#digital-forensics-examiner) | Collects and analyzes digital evidence (often for legal cases) |
  | [Malware Analyst](#malware-analyst) | Reverse-engineers malicious programs (static + dynamic analysis) |
  | [Penetration Tester](#penetration-tester) | Ethically hacks systems to find vulnerabilities and report risks |
  | [Red Teamer](#red-teamer) | Emulates real threat actors; tests detection and response capabilities |

---

#### Security Analyst ####
"Security analysts construct security measures to protect the company from attacks. Analysts explore and evaluate company networks to uncover actionable data." - THM

**Responsibilities**
- Working with various stakeholders to analyse the cyber security throughout the company.
- Compile ongoing reports about the safety of networks, documenting security issues and measures taken in response.
- Develop security plans, incorporating research on new attack tools and trends, and measures needed across teams to maintain data security.

#### Security Engineer ####
"Security engineers develop and implement security solutions."

**Responsibilities**
- Testing and screening security measures across software
- Monitor networks and reports to update systems and mitigate vulnerabilities
- Identify and implement systems needed for optimal security

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

#### Red Teamer ####
Red teamers share similarities to penetration testers, with a more targeted job role. 

**Responsibilities**
- Emulate the role of a threat actor to uncover exploitable vulnerabilities, maintain access and avoid detection
- Assess organisations' security controls, threat intelligence, and incident response procedures
- Evaluate and report on insights, with actionable data for companies to avoid real-world instances

**End of Room 3**

</details>

---

**End of Module 1**

</details>

---














<details><summary><strong>Module 2 - Computer Fundamentals</strong></summary>
  
## Module 2 - Computer Fundamentals

<details><summary><strong>Room 1 - Inside a Computer System</strong></summary>
  
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

**End of Room 1**

</details>

---

<details><summary><strong>Room 2 - Computer Types</strong></summary>
  
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

**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - Client-Server Basics</strong></summary>
  
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

**End of Room 3**

</details>

---

<details><summary><strong>Room 4 - Virtualization Basics</strong></summary>

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

**Containers**\
A container is a lightweight, isolated environment that packages a single application + everything it needs (libraries, tools, versions).

**Key characteristics:**
- Shares the host operating system (much lighter than a full VM)
- Starts almost instantly
- Stays isolated from other containers
- Runs the same way on any machine → perfect for development, testing, and scaling

**Quick comparison**
- **VM** = full virtual computer (own OS)
- **Container** = just the application + its dependencies (shares the host OS)

**End of Room 4**

</details>

---

<details><summary><strong>Room 5 - Cloud Computing Fundamentals</strong></summary>

### Room 5 - Cloud Computing Fundamentals

**The Problem with Self-Hosting**\
Hosting an app on your own computer means:
- Sharing your IP address (hard to remember, especially IPv6)
- Keeping the computer online 24/7
- Limited capacity when traffic grows
- Difficult to scale or reach a large audience

**Cloud computing** solves these issues.

**Learning Objectives**
- What cloud computing is
- Service models: IaaS, PaaS, SaaS
- Cloud types: Public, Private, Hybrid
- Benefits of cloud computing
- How major companies use the cloud

**Key Benefits & Characteristics**
- **Scalability** – easily add or remove resources as demand changes
- **On-demand self-service** – create/remove servers and storage instantly
- **Pay-as-you-go** – charged only for what you actually use
- **Security** – providers handle strong infrastructure protection
- **High availability** – apps keep running even if parts of the system fail
- **Global access** – users can reach your app from anywhere

**Types of Cloud**
<div>

  | **Type** | **Typical Users**                | **Why it's used**                                  |
  |----------|----------------------------------|----------------------------------------------------|
  | Public   | Startups, websites, global apps  | Affordable, easy to scale, no hardware to manage   |
  | Private  | Banks, healthcare, government    | Greater control, customization, and compliance     |
  | Hybrid   | E-commerce and similar companies | Keep sensitive data private while scaling publicly |
  
</div>

**Cloud Service Models**
<div>

  | **Model** | **Full Name**               | **What you manage**   | **What the provider manages**         | **Example use**                      |
  |-----------|--------------------|------------------|--------------------|-----------------|
  | IaaS      | Infrastructure as a Service | OS + application      | Physical hardware, virtualization     | Virtual servers, storage, networking |
  | PaaS      | Platform as a Service       | Your application only | Infrastructure + OS                   | Focus on building and deploying apps |
  | Saas      | Software as a Service       | Nothing (just use it) | Everything                            | Gmail, Zoom, etc.                    |
  
</div>

**Major Cloud Vendors**
- **AWS (Amazon Web Services)** – broadest range of services, pay-as-you-go
- **Microsoft Azure** – strong in enterprise and hybrid environments
- **Google Cloud Platform (GCP)** – strong in data analytics, AI, and machine learning
- **Alibaba Cloud** – major player in Asia, growing globally
- **IBM Cloud** – hybrid cloud and AI-focused solutions
- **Oracle Cloud** – enterprise applications and databases


**End of Room 5**

</details>

---

**End of Module 2**

</details>

---












<details><summary>Module 3 - Operating Systems Basics<strong></strong></summary>

## Module 3 - Operating Systems Basics

<details><summary><strong>Room 1 - Operating Systems - Introduction</strong></summary>

### Room 1 - Operating Systems - Introduction
**Learning Objectives**
- Understand what an operating system is and the role it plays
- Explain the core duties of an operating system
- Identify common OS types and their typical use cases
- Practice interacting with an OS to gather system information

**Key Terminology**
- Operating System (OS)
- Kernel space
- User space
- Graphical User Interface (GUI)
- Command-Line Interface (CLI)

---

#### What is an Operating System?

The operating system is the core software that coordinates everything happening on a computer. It acts as the middleman between the hardware and the applications we use.

**User Applications → Operating System → Hardware**

Without an OS, every application would need direct control over the CPU, memory, files, devices, and security. This separation is intentional and helps prevent conflicts and security issues.

- **Kernel space**: The privileged, locked-down core of the OS. It has unrestricted access to the hardware.
- **User space**: Where all standard applications run.

---

#### Operating System Duties

Every OS is responsible for a few core duties that allow your computer to run safely, efficiently, and predictably.

| OS Responsibility       | What the OS Does                                      | Example                                      |
|-------------------------|-------------------------------------------------------|----------------------------------------------|
| Process Management      | Creates, schedules, prioritizes, and terminates programs | Opening multiple apps at the same time      |
| Memory Management       | Allocates RAM to processes and protects their memory  | Isolating each open app’s memory             |
| File System Management  | Organizes files, handles paths, permissions, and metadata | Creating folders, saving files, setting permissions |
| User Management         | Handles accounts, authentication, and permissions     | Logging in with a username and password      |
| Device Management       | Loads drivers and provides a universal interface      | Plugging in a mouse, printer, or external drive |

---

#### Operating System Security

At a basic level, the operating system handles:
- **Authentication** — Verifies who you are (passwords, biometrics)
- **Permissions** — Controls what each user and application can read, write, or execute
- **Isolation** — Keeps every process in its own protected space (kernel vs user space)
- **System Protection** — Safeguards critical system files and settings

**Interfaces**
- **Graphical User Interface (GUI)**: Visual representation of information
- **Command-Line Interface (CLI)**: Text-based interface for entering commands

---

#### Types of Operating Systems

| OS Type          | Primary Use Case                          | Key Characteristics                              |
|------------------|-------------------------------------------|--------------------------------------------------|
| Desktop          | Personal computers, daily work, gaming    | Rich graphical interface                         |
| Server           | Web hosting, databases, cloud services    | Headless, high uptime, multi-user, remote access |
| Mobile           | Smartphones and tablets                   | Touch-based, power efficient, app sandboxing     |
| Embedded         | Appliances, cars, IoT devices             | Tiny footprint, limited hardware                 |
| Virtual / Cloud  | Labs, containers, cloud instances         | Lightweight, scalable, rapid deployment          |

---

#### Real-World Operating Systems

**Desktop**
- **Windows**: Most widely used on personal computers (Windows 10, Windows 11)
- **macOS**: Apple’s desktop OS known for its polished interface (Sonoma, Sequoia)
- **Linux**: Family of open-source distributions (Ubuntu, Debian, Fedora)

**Server**
- **Windows Server**: Used in corporate environments and data centers (2019, 2022, 2025)
- **Linux**: Powers the majority of web servers (Ubuntu Server, Debian, CentOS, Red Hat)
- **Unix**: Used in large enterprises (IBM AIX, Oracle Solaris)

**Mobile**
- **Android**: Most widely used mobile OS
- **iOS**: Apple’s mobile operating system

**Embedded & IoT**
- Embedded Linux (OpenWrt, Ubuntu Core, Yocto)
- Real-Time OS (FreeRTOS, VxWorks, QNX)

**Virtual & Cloud**
- Cloud/VM: Ubuntu LTS, Amazon Linux, Rocky Linux
- Container-optimized: Alpine Linux, Bottlerocket, Flatcar

---

**Further Learning** (Official Links)
- [Windows Basics](https://tryhackme.com/room/windowsbasics)
- [Linux CLI Basics](https://tryhackme.com/room/linuxclibasics)
- [Windows CLI Basics](https://tryhackme.com/room/windowsclibasics)


**End of Room 1**

</details>

---

<details><summary><strong>Room 2 - Windows Basics</strong></summary>


### Room 2 - Windows Basics
**Learning Objectives**
- Navigate the Windows graphical interface (desktop, taskbar, and Start menu)
- Use File Explorer to browse folders, understand file paths, and organize files
- Check system settings and personalize the Windows environment using the Settings app
- Use basic system tools like Task Manager and Windows Security to monitor performance and verify protection

---

#### Exploring the Windows Workspace

Before accessing the Windows desktop, you must **authenticate** (prove your identity). Authentication determines what actions you are allowed to take once logged in.

**Typical Account Types**
- **Guest** — Restricted account for temporary access with minimal permissions
- **Standard** — Everyday user account; cannot make system-wide changes
- **Administrator** — Privileged account with full control over the system

---

#### Core Desktop Components
- **Desktop** — Main workspace for files, folders, and shortcuts
- **Taskbar** — Control strip that provides access to applications, system tools, settings, and notifications

**Key Features**
1. **Desktop icons** — Shortcuts to the Recycle Bin, folders, and frequently used applications (fully customizable)
2. **Start menu** — Primary way to access applications, settings, and power options
3. **Search** — Quickly find applications, files, folders, and settings
4. **Task View** — View and switch between all open windows
5. **Pinned applications** — Quick access to your most-used apps and folders
6. **Network & Audio settings** — System status and quick controls
7. **Date and Time** — Calendar and time settings
8. **Notifications** — System and application alerts

---

#### Updating Applications

Keeping your operating system and applications up to date is essential for security and stability.

**Windows Updates**
- Windows has a built-in **Windows Update** tool that keeps the OS and many native applications current.

**Application Updates**
- Built-in apps may update automatically
- Third-party apps often include their own update mechanisms
- Some apps prompt you to update on launch
- Others require manual checking or downloading a new installer

**Installing Applications**
1. **Microsoft Store** — Curated and safer option (not available by default on Windows Server)
2. **From the Internet** — Download `.exe` or `.msi` installers from trusted vendor websites

**Uninstalling Applications**
- Microsoft Store (for apps installed from the Store)
- **Settings → Apps → Installed apps**
- Control Panel → Programs and Features
- Application’s built-in uninstaller

---

#### Diving Into Settings

Windows provides two main interfaces for configuration:

1. **Windows Settings** — Modern, centralized location for system, device, personalization, and security settings
2. **Control Panel** — Legacy interface still used for certain administrative tasks

---

#### Task Manager

Task Manager is a built-in tool that lets you monitor system activity in real time.

**Main Tabs**
1. **Processes** — Currently running apps and background processes with resource usage
2. **Performance** — Graphs for CPU, memory, disk, and network
3. **Users** — Currently logged-in users and their resource usage
4. **Details** — Technical view of processes, including Process IDs (PIDs)
5. **Services** — Windows services and their current status (running or stopped)

---

#### Native Windows Security

**Windows Security** is the central dashboard for managing built-in protection.

**Main Sections**
- **Virus & threat protection** — Real-time protection and scans for malware
- **Firewall & network protection** — Controls network traffic
- **App & browser control** — Protects against unsafe apps, files, and websites
- **Device security** — Hardware-based protections

**Windows Defender Firewall Network Profiles**
- **Domain** — Used on organizational domain networks
- **Private** — Trusted networks (home or lab)
- **Public** — Untrusted networks (public Wi-Fi)

In **Advanced settings** you can view and manage:
- Inbound, outbound, and connection security rules
- Detailed rule information (name, group, profile, status, action)
- Create or filter rules


**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - Linux CLI Basics</strong></summary>


### Room 3 - Linux CLI Basics
**Learning Objectives**
- Understand what the Linux terminal is and what it’s used for
- Feel comfortable interacting with the Linux environment
- Navigate the Linux filesystem using basic commands

---

#### A Quick Note About the Terminal

The **terminal** is a text-based interface for controlling a Linux system. Instead of clicking through a graphical interface, you type commands that tell the computer exactly what to do.

Cybersecurity professionals prefer the terminal because:
- It’s faster than clicking around
- It gives more precise control
- Many security tools only run in the terminal

---

#### Interacting With the Terminal

**Step 1: Where am I?**
- *pwd* - Shows the current working directory (Present Working Directory).

**Step 2: What’s around me?**
- *ls*          - List files and folders
- *ls -l*       - Detailed list (permissions, size, date)
- *ls -al*      - Includes hidden files (those starting with .)

Step 3: Let’s move around
- *cd*     - Change directory
- *cd ..*  - Moves up one directory

**Step 4: Find files**
- *find <starting_point> -name <filename>*
- **Example:** find / -name "passwd"

**Step 5: Read a file**
- *cat <filename>*

---

#### Investigating the System

**Step 1: Who are you logged in as?**
- *whoami*

**Step 2: What system are you on?**
- *uname -a*      - Displays kernel and system information.

**Step 3: Check disk and storage info**
- *df -h*
  - /dev/root → Main system disk
  - tmpfs → Temporary filesystems stored in RAM
  - /dev/shm → Shared memory area
  - /run/user/... → Temporary storage for user sessions

**Step 4: Read a system file**\
Linux stores important configuration and informational files in the /etc directory.\
**Example:** cat /etc/passwd

**End of Room 3**

</details>

---

<details><summary><strong>Room 4 - Windows CLI Basics</strong></summary>


### Room 4 - Windows CLI Basics

**Learning Objectives**
- Use the Windows command line confidently
- Navigate folders without clicking
- Find files when you only know their name
- Read files using the terminal
- Collect basic system and network information

---

#### What is the Windows Command Line?

The **Command Prompt** (CMD) is a text-based interface for interacting with the Windows operating system. Instead of clicking folders and menus, you type commands to tell the system exactly what to do.

Cybersecurity professionals use the command line because:
- It’s faster than clicking around
- It gives more precise control
- Many security tools only run in the terminal

---

#### Navigating Files and Finding a File

**Step 1: Where am I?**
- *cd* - Shows your current location (Current Directory).

**Step 2: What’s around me?**
- *dir* - Lists files and folders in the current directory.

**Step 3: Are there hidden files?**
- *dir /a* - Shows all files, including hidden ones.

**Step 4: Moving around the filesystem**
- *cd <folder_name>*     - Move into a folder
- *cd ..*                - Move up one level

**Step 5: Finding a file on the disk**
- *dir /s <filename>* - Searches all subdirectories for the specified file name.

**Step 6: Navigate to the file**
- *cd <path_to_file>*

**Step 7: Read the file**
- *type <filename>*

---

#### Gathering System Information on Windows

**Step 1: Who am I logged in as?**
- *whoami*

**Step 2: What is the name of this computer?**
- *hostname*

**Step 3: What version of Windows is this?**
- *systeminfo*

**Step 4: How is this machine connected to the network?**
- ipconfig

**End of Room 4**

</details>

---

<details><summary>Room 5 - Operating System Security<strong></strong></summary>


### Room 5 - Operating System Security

**Learning Objectives**
- Understand the importance of operating system security
- Identify common security weaknesses in operating systems
- Apply basic security concepts such as authentication, permissions, and protection against malicious software

---

#### Introduction to Operating System Security

An **operating system (OS)** sits between the hardware and the applications you run. It controls access to the CPU, memory, storage, and devices.

Because modern devices (phones, laptops, servers) store a large amount of private and sensitive data, securing the operating system is critical.

When we talk about security, we protect three main principles (the **CIA Triad**):
- **Confidentiality** — Only authorized people can access the data
- **Integrity** — Data cannot be modified without authorization
- **Availability** — Systems and data are available when needed

---

#### Common Examples of OS Security Issues

**1. Authentication and Weak Passwords**\
Authentication verifies identity using:
- Something you **know** (password or PIN)
- Something you **are** (fingerprint, biometrics)
- Something you **have** (phone for SMS codes)

#### Common Weak Passwords

Many people still use very weak and predictable passwords. The **RockYou** breach (2009) exposed millions of passwords and is still commonly used in password attacks today.

**Top 10 most common passwords from RockYou:**

 | **Rank** | **Password**|
 |----------|-------------|
 | 1.       | 123456      |
 | 2.       | 12345       |
 | 3.       | 123456789   |
 | 4.       | password    |
 | 5.       | iloveyou    |
 | 6.       | princess    |
 | 7.       | rockyou     |
 | 8.       | 1234567     |
 | 9.       | 12345678    |
 | 10.      | abc123      |

**2. Weak File Permissions**\
The **principle of least privilege** states that users and programs should only have the minimum access needed to perform their tasks.

Weak permissions can allow attackers to:
- Read confidential files (Confidentiality)
- Modify or delete files (Integrity)

**3. Malicious Programs**\
Malware can attack all three parts of the CIA Triad:
- **Trojans** — Give attackers remote access
- **Ransomware** — Encrypts files and demands payment (Availability)

---

#### Practical Concepts Demonstrated

In the practical portion of the room, the following concepts were applied:

- Using **SSH** to remotely access a Linux system
- Switching between user accounts
- Exploiting weak passwords
- Viewing command history
- Escalating privileges to the `root` (administrator) account

These steps highlight why strong passwords, proper user privileges, and careful system configuration are essential for OS security.

**End of Room 5**

</details>

---

**End of Module 3**

</details>

---











<details><summary><strong>Module 4 - Software Basics</strong></summary>

## Module 4 - Software Basics

<details><summary><strong>Room 1 - Data Representation</strong></summary>

### Room 1 - Data Representation


**End of Room 1**

</details>

---

<details><summary><strong>Room 2 - Data Encoding</strong></summary>


### Room 2 - Data Encoding


**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - Python - Simple Demo</strong></summary>

### Room 3 - Python - Simple Demo


**End of Room 3**

</details>

---

<details><summary><strong>Room 4 - JavaScript - Simple Demo</strong></summary>

### Room 4 - JavaScript - Simple Demo


**End of Room 4**

</details>

---

<details><summary><strong>Room 5 - Database SQL Basics</strong></summary>

### Room 5 - Database SQL Basics


**End of Room 5**

</details>

---

**End of Module 4**

</details>

---











<details><summary><strong>Module 5 - Network Fundamentals</strong></summary>

## Module 5 - Network Fundamentals

<details><summary><strong>Room 1 - What is Networking</strong></summary>

### Room 1 - What is Networking


**End of Room 1**

</details>

---



<details><summary><strong>Room 2 - Intro to LAN</strong></summary>

### Room 2 - Intro to LAN


**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - OSI Model</strong></summary>

### Room 3 - OSI Model


**End of Room 3**

</details>

---

<details><summary><strong>Room 4 - Packets and Frames</strong></summary>

### Room 4 - Packets and Frames


**End of Room 4**

</details>

---

<details><summary><strong>Room 5 - Extending Your Network</strong></summary>

### Room 5 - Extending Your Network


**End of Room 5**

</details>

---

**End of Module 5**

</details>

---













<details><summary><strong>Module 6 - How The Web Works</strong></summary>

## Module 6 - How The Web Works

<details><summary><strong>Room 1 - DNS in Detail</strong></summary>

### Room 1 - DNS in Detail


**End of Room 1**

</details>

---

<details><summary><strong>Room 2 - HTTP in Detail</strong></summary>

### Room 2 - HTTP in Detail


**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - How Websites Work</strong></summary>

### Room 3 - How Websites Work


**End of Room 3**

</details>

---

<details><summary><strong>Room 4 - Putting it all together</strong></summary>

### Room 4 - Putting it all together


**End of Room 4**

</details>

---

**End of Module 6**

</details>

---


















<details><summary><strong>Module 7 - Attacks and Defense</strong></summary>

## Module 7 - Attacks and Defense

<details><summary><strong>Room 1 - The CIA Triad</strong></summary>

### Room 1 - The CIA Triad


**End of Room 1**

</details>

---

<details><summary><strong>Room 2 - Cryptography Concepts</strong></summary>

### Room 2 - Cryptography Concepts


**End of Room 2**

</details>

---

<details><summary><strong>Room 3 - Become a Hacker</strong></summary>

### Room 3 - Become a Hacker


**End of Room 3**

</details>

---

<details><summary><strong>Room 4 - Become a Defender</strong></summary>

### Room 4 - Become a Defender


**End of Room 4**

</details>

---

**End of Module 7**

</details>


---


<!-- End of File -->




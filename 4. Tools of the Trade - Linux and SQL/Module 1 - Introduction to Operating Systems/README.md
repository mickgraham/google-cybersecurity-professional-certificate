# Module 1: Introduction to Operating Systems

## Overview

* Common operating systems
* Main functions of an operating system
* Virtualization technology
* Graphical user interfaces and command-line interfaces

## Common operating systems

An operating system (OS) is the interface between computer hardware and the user.

* **Windows and macOS:** Are both common operating systems. The Windows operating system was introduced in 1985, and macOS was introduced in 1984. Both operating systems are used in personal and enterprise computers.
* **Linux:** The first version of Linux was released in 1991, and other major releases followed in the early 1990s. Linux is a completely open-source operating system, which means that anyone can access Linux and its source code. The open-source nature of Linux allows developers in the Linux community to collaborate.
* **ChromeOS:** Launched in 2011. It's partially open source and is derived from Chromium OS, which is completely open source. ChromeOS is frequently used in the education field.
* **Android and iOS:** Are both mobile operating systems. Unlike the other operating systems mentioned, mobile operating systems are typically used in mobile devices, such as phones, tablets, and watches. Android was introduced for public use in 2008, and iOS was introduced in 2007. Android is open source, and iOS is partially open source.

### Operating systems and vulnerabilities

Security issues are inevitable with all operating systems. An important part of protecting an operating system is keeping the system and all of its components up to date.

* **Legacy operating systems:** Are operating systems that are outdated but still being used. Some organizations continue to use legacy operating systems because software they rely on is not compatible with newer operating systems.

Legacy operating systems can be vulnerable to security issues because they're no longer supported or updated. This means that legacy operating systems might be vulnerable to new threats.

## Main functions of an operating system

### Booting the computer

When you boot, or turn on, your computer, either a BIOS or UEFI microchip is activated.

* The **Basic Input/Output System (BIOS)** is a microchip that contains loading instructions for the computer and is prevalent in older systems.
* The **Unified Extensible Firmware Interface (UEFI)** is a microchip that contains loading instructions for the computer and replaces BIOS on more modern systems.

The last instruction from the BIOS or UEFI activates the bootloader. The bootloader is a software program that boots the operating system. Once the operating system has finished booting, your computer is ready for use.

### Completing a task

Once a computer has gone through the booting process, completing a task on a computer is a four-part process.

![User, Application, Operating-System, Hardware](user-application-operating-system-hardware.png)

### The OS at work behind the scenes

An example: Downloading a file from an internet browser:

* First, the user decides they want to download a file that they found online, so they click on a download button near the file in the internet browser application.
* Then, the internet browser communicates this action to the OS.
* The OS sends the request to download the file to the appropriate hardware for processing.
* The hardware begins downloading the file, and the OS sends this information to the internet browser application. The internet browser then informs the user when the file has been downloaded.

## Virtualization technology

A **virtual machine (VM)** is a virtual version of a physical computer. Virtual systems don't use dedicated physical hardware. Instead, they use software-defined versions of the physical hardware. This means that a single virtual machine has a virtual CPU, virtual storage, and other virtual hardware. Virtual systems are just code. You can run multiple virtual machines using the physical hardware of a single computer. This involves dividing the resources of the host computer to be shared across all physical and virtual components.

There are many benefits to using virtual machines, such as isolation of malware and other security risks. However, it's important to remember there's still a risk of malicious software escaping their virtualized environments.

### Benefits of virtual machines

Security professionals commonly use virtualization and virtual machines. Virtualization can increase security for many tasks and can also increase efficiency.

* **Security:** Virtualization provides an isolated environment on a host machine, allowing security professionals to safely test or contain malware, though risks remain if a malicious program escapes the virtual environment.
* **Efficiency:** Using virtual machines allows multiple instances to run on a single physical machine, similar to how a city bus efficiently transports many people compared to each person driving separately.

## Graphical user interfaces and command-line interfaces

A graphical user interface (GUI) is a user interface that uses icons on the screen to manage different tasks on the computer. A command-line interface (CLI) is a text-based user interface that uses commands to interact with the computer.

One notable difference between these two interfaces is how they appear on the screen. A GUI has graphics and icons, such as the icons on your desktop or taskbar for launching programs. In contrast, a CLI only has text. It looks similar to lines of code.

These two interfaces also differ in how they function. A GUI is an interface that only allows you to make one request at a time. However, a CLI allows you to make multiple requests at a time.

When working in cybersecurity, a CLI is often preferred over a GUI because it can handle multiple tasks simultaneously and it includes a history file.

## Glossary: Introduction to Operating Systems

**Application:** A program that performs a specific task

**Basic Input/Output System (BIOS):** A microchip that contains loading instructions for the computer and is prevalent in older systems

**Bootloader:** A software program that boots the operating system

**Command-line interface (CLI):** A text-based user interface that uses commands to interact with the computer

**Graphical user interface (GUI):** A user interface that uses icons on the screen to manage different tasks on the computer

**Hardware:** The physical components of a computer

**Legacy operating system:** An operating system that is outdated but still being used

**Operating system (OS):** The interface between computer hardware and the user

**Random Access Memory (RAM):** A hardware component used for short-term memory

**Unified Extensible Firmware Interface (UEFI):** A microchip that contains loading instructions for the computer and replaces BIOS on more modern systems

**User interface:** A program that allows the user to control the functions of the operating system

**Virtual machine (VM):** A virtual version of a physical computer

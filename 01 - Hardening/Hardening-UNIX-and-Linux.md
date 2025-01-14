# Hardening Linux

Hardening UNIX and Linux largely comes from the combination of the administration guides, user manuals, and experience in the security world. Various certifications have different standards for hardening operating systems like Linux into configurations that are resilient to cybersecurity attacks.

In Linux there are many many manuals which may be present. Depending on which version of Linux you are dealing with; you will have different security implementation for the same surface area. Different versions of the TCP/IP stack in Linux change over time. As do the service management part of the operating system. Scheduled jobs and other dynamic parts of the operating system have also had a few changes over time.

Since the early days in UNIX systems, most cybersecurity came down to firewalls and file permissions and service configurations. Hardening against the ATT&CK and CAPEC standards for different Linux systems is important. Being resilient to any attack which is possible in DragOS or Kali Linux may not be possible at different times for the same system. Research lifts veils of secrecy on operations of malware. And the landscape evolves as developers change their code with the operating system.

Locking down anything that can be locked down is a good practice. Layered security is also an important concept. The practice of enforcing Linux security is vastly flexible and majorly dependent on the system implementation for which the computer is being used. There are various types of security which may be possible or employed while securing your operating system. Different operating systems support different features. Disk encryption may be different for certain operating systems.

The CMMC model for cloud computing is one which is largely accepted for security practices on hardening Linux. Various container services are configured to match this compliance level. ISO, NIST, SANS, EC-Council, CompTIA and other bodies of authority voice that reduction of surface area, principles of least priviledge, and strong encryption standards are a strong way of going about cybersecurity.

The process is largely straight forward. The following is a simple idea. Secure the system. This process does not capture everything that an Administration Guide, or Reference Manual may encompass; but this is some of what it boils down to in Linux.

1. Securely build or download your installation medium
2. Prepare the hardware for installation to organization standards
3. Ensure firmware, BIOS, and all other supporting firmware, software, wetware are within risk tolerance
3a. Authenticate the hardware to the network
3b. Generate accounts for MFA and PRNG paired tokens and similar infrastructure
4. Install the operating system with minimal configuration
4a. If possible, isolate partitions to separate system and user spaces
4b. If possible, create user accounts specifically for locked down resources
4c. If possible or necessary, encrypt the disk with LUKS or appropriate encryption
4d. Install the system from an approved mirror and do not install superfluous packages
4e. Do not generate unecessary traffic which may result in MitM traffic during the install
5. Once installed, start locking down the system
8. Configure the firewall for necessary communication
6. Make sure the system is up to date
7. Install and configure SELinux if necessary
7a. Create contexts, labels, and ACLs associated with your systems needs
7b. If the system is a web server, enable web-specific SELinux features
8. Begin reducing noise in the operating system
8a. Disable unecessary services 
8b. Disable unecessary kernel options, modules, networking capabilities
8c. Disable unecessary logging rules
8d. Disable unecessary operating system features
8e. Switch compositor, graphics libraries, desktop environment to approved secure resource standards
8f. Disable unecessary network services 
8g. Disable unecessary language compiler or runtime support
8e. Disable uneccesary repositories and network repositories and use appropriate mirrors
8f. If possible switch to internal approved repositories and mirrors
8g. If possible implement a DNS filtering policy
8h. Disable uneccessary networking protocols at the kernel and firewall level
8i. Switch to approved time servers
9. Implement auditing trails and logging features
9a. Configure logging and audit policies for the kernel, operating system, and applications
9b. Standardize logging data format for easier digestion in automated services
10. Modify user accounts to use ZTA or Least Privilege capability models
11. Reduce LOLbin surface area by locking tools behind user accounts, policies, credentials, and sudo
12. Apply STIG configurations
13. Determine SCAP patching level
14. Mature to CMMC and 800-53 standards.  

## Linux Kernel Documentation

https://docs.kernel.org/

### Linux Kernel User's adn Administrator's Guide

https://docs.kernel.org/admin-guide/index.html

# Linux Administrator's Guides

## Fedora Linux

### Fedora Linux Documentation 

https://docs.fedoraproject.org/en-US/docs/

### Fedora Linux User Documentation

https://docs.fedoraproject.org/en-US/fedora/latest/

### Fedora System Administrator's Guide

https://docs.fedoraproject.org/en-US/fedora/f40/system-administrators-guide/

## RedHat Linux

### RedHat Administrator's Guide

### Hardening Red Hat Enterprise Linux

https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/8/html/security_hardening/index

### RedHat RHEL Linux | SELinux User's and Administrator's Guide

https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/7/html/selinux_users_and_administrators_guide/index

## OpenSolaris and Solaris 

https://docs.oracle.com/cd/E18752_01/html/817-1985/index.html

## openSUSE

### openSUSE Security and Hardening Guide

https://doc.opensuse.org/documentation/leap/security/html/book-security/index.html

## Debian Linux

### Debian User Manuals

https://www.debian.org/doc/user-manuals

#### Debian Administrator's Handbook

https://packages.debian.org/debian-handbook

### Chapter 14. Security | Debian Administrator's Handbook

https://www.debian.org/doc/manuals/debian-handbook/security.en.html

## Ubuntu Server Documentation

https://ubuntu.com/server/docs

## Arch Linux 

### Arch Linux | User Documentation

https://wiki.archlinux.org/title/Category:System_administration

### Arch Linux | Security Category 

https://wiki.archlinux.org/title/Category:Security

## OpenBSD 

https://www.openbsdhandbook.com/

### OpenBSD Handbook Networking Guide

https://www.openbsdhandbook.com/networking/

### Hardened Linux from Scratch

https://www.linuxfromscratch.org/hlfs/download.html

### Gentoo Security Handbook

https://wiki.gentoo.org/wiki/Security_Handbook

### Linux Network Administrator's Guide

https://tldp.org/LDP/nag2/nag2.pdf

### Cygwin User Guide

https://www.cygwin.com/cygwin-ug-net.html

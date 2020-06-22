# TryHackMe-RP-Nessus-Write-Up
Part of the Red Primer series, learn how to set up and use Nessus.

## [Task 1] Deploy!

Deploy the vulnerable machine! This one, well, it has problems.

### #1 	Deploy the virtual machine!

No answer needed

## [Task 2] Installation

### #1 	First, create a basic Ubuntu box (or any other system of your choice). Minimum 4 2GHz cores, 4 GB RAM (8 Recommended) and 30 GB of disk space.

No answer needed

### #2 	Next, go ahead and register for a Nessus Home license. This can be used to scan up to 16 IP addresses at a time. Be sure to keep this license information safe, you'll need it for any manual work. Here's the registration link: https://www.tenable.com/products/nessus-home

No answer needed 

### #3 	Follow the installation instructions on Tenable's website, once Nessus is set up connect the machine that it lives on to the network using your VPN file.

No answer needed 

## [Task 3] Nessus Quiz

### #1 	As we log into Nessus, we are greeted with a button to launch a scan, what is the name of this button?

answer: New Scan

### #2 	Nessus allows us to create custom templates that can be used during the scan selection as additional scan types, what is the name of the menu where we can set these?

answer: Policies

### #3  Nessus also allows us to change plugin properties such as hiding them or changing their severity, what menu allows us to change this?

answer: Plugin Rules

### #4 	Nessus can also be run through multiple 'Scanners' where multiple installations can work together to complete scans or run scans on remote networks, what menu allows us to see all of these installations?

Answer: Scanners

### #5 	Let's move onto the scan types, what scan allows us to see simply what hosts are 'alive'?

Answer: Host Discovery

### #6 	One of the most useful scan types, which is considered to be 'suitable for any host'?

Answer: Basic Network Scan

### #7 	Following a few basic scans, it's often useful to run a scan wherein the scanner can authenticate to systems and evaluate their patching level. What scan allows you to do this?

Answer: Credentialed Patch Audit

### #8 	When performing Web App tests it's often useful to run which scan? This can be incredibly useful when also using nitko, zap, and burp to gain a full picture of an application. 

Answer: Web Application Tests

## [Task 4] Scanning!

Run a basic network scan and learn to read through the results!

### #1 	Deploy the machine and connect to the network

No answer needed

### #2 	Create a new 'Basic Network Scan' targeting the deployed VM. What option can we set under 'BASIC' to set a time for this scan to run? This can be very useful when network congestion is an issue.

answer: Schedule

### #3  Under discovery set the scan to cover ports 1-65535. What is this type called?

answer: Port scan (all ports)

### #4 	As we are connected to the network via a VPN, it may be to our benefit to 'tone down' the scan a bit. What scan type can we change to under 'ADVANCED' for this lower bandwidth connection?

Answer: Scan low bandwidth links

### #5 	With these options set (other than the time to run) save and launch the scan.

No answer needed

### #6 	After the scan completes, which 'Vulnerability' can we view the details of to see the open ports on this host?

Answer: Nessus SYN scanner

### #7 	There seems to be a chat server running on this machine, what port is it on?

Answer: 6667

### #8 	Looks like we have a medium level vulnerability relating to SSH, what is this vulnerability named? 

Answer: SSH Weak Algorithms Supported

### #9 	What web server type and version is reported by Nessus?

Answer: Apache/2.4.99




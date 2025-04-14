##Project Title:
Mapping Hostnames to IPv4 Addresses Using a Python Script

##Intended Audience:
This project is part of a Product Assessment for the Cyber Security course.

##Project Objective and Requirements:
The objective of this project is to develop a Python script that maps a list of user-entered hostnames to their corresponding IPv4 addresses.

Functionality Overview:
- The script prompts the user to enter a series of hostnames.
- Input is terminated when the user presses Enter on an empty line.
- The script displays a numbered list (starting from 0) of the entered hostnames.
- The user is then prompted to select a hostname by its index.
- The script resolves and displays the corresponding IPv4 address for the selected hostname.
- Pressing Enter on an empty line at this stage will also terminate the script.

Error Handling:
- The script will terminate and display appropriate error messages in the following scenarios:
- No hostnames were entered.
- An invalid index was entered (e.g., a number outside the list range, or a non-integer value).
- The selected hostname could not be resolved to an IP address.

##Development Environment:

- Operating System: Windows
- IDE/Text Editor: Visual Studio Code
- Programming Language: Python 3.11

##Required Library:
socket (Standard Python Library)

Purpose:
The socket library enables low-level networking operations and is used to resolve hostnames to their respective IPv4 addresses using the function:
socket.gethostbyname(hostname)

##Data Structure Used:
List: A list is used to store the entered hostnames. Lists in Python can hold multiple data types and allow indexed access to elements.

##Getting Started:
1. Running the Script:
Launch the script in your Python environment.

2. Entering Hostnames:
You will be prompted to enter hostnames. Press Enter on an empty line to complete the input.
Example:

www.google.com  
www.facebook.com  
www.rmit.edu.au  

3.Selecting a Hostname:
After entering hostnames, the script will display them with indices:

0. www.google.com  
1. www.facebook.com  
2. www.rmit.edu.au

4. Enter the index of the desired hostname to retrieve its IPv4 address.
Example:
Please enter the number of the desired hostname: 1  
IPv4 address for host www.facebook.com is 157.240.8.35

5. Terminating the Script:

- Press Enter on an empty line during index selection to exit.
- The script also exits automatically after displaying the IP address or if any error is encountered.


# Port-Scanner
## Introduction
This Python script is a simple yet effective tool for scanning open ports on a given IP address. Whether you're a network administrator or a cybersecurity enthusiast, this port scanner can help you identify potential vulnerabilities by checking which TCP ports are open on your target machine.
## Features
Easy to Use: Just input the IP address and the range of ports you want to scan.
Fast and Efficient: Uses Python's socket module for rapid scanning.
Configurable Port Range: Allows scanning of specific port ranges based on user input.
## Installation
To use this port scanner, you need Python installed on your machine. Clone this repository to your local machine using the following command:
```ps 
git clone https://github.com/pourjavadi/Port-Scanner.git
```
Navigate to the directory where you cloned the repo:
```ps
cd port-scanner
```
## Usage
Run the script by executing the following command in your terminal:
```ps
python port-scanner.py
```
Follow the on-screen prompts to enter the IP address and the range of ports you want to scan. The script will output a list of open ports.

Examples
Here's an example of how to run the script:
```ps
Please enter the IP address: 192.168.1.1
Enter the start port number (e.g., 1): 1
Enter the end port number (e.g., 1024): 1024
```
The script will then perform the scan and display any open ports.

Contributing
Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to fork the repository and submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

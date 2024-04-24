# Port-Scanner
port scanner

import socket

def scan_ports(ip, start_port, end_port):
    open_ports = []
    for port in range(start_port, end_port + 1):
        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
        sock.settimeout(1)  # Set timeout for the connection
        result = sock.connect_ex((ip, port))
        if result == 0:
            open_ports.append(port)
        sock.close()
    
    return open_ports

# Getting user input
ip_address = input("Please enter the IP address: ")
start_port = int(input("Enter the start port number (e.g., 1): "))
end_port = int(input("Enter the end port number (e.g., 1024): "))

# Executing port scan
open_ports = scan_ports(ip_address, start_port, end_port)

# Displaying results
if open_ports:
    print("Open ports:")
    for port in open_ports:
        print(port)
else:
    print("No open ports found.")

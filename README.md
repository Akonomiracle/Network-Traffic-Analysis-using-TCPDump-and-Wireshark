# Network Traffic Analysis Tool using TCPDump and Wireshark

## Objective

Developed a tool for capturing and analyzing network traffic using TCPDump. The tool was built with features like saving captured packets, creating sequenced dump files, and decrypting SSL/TLS traffic with Wireshark. I used shell scripting to automate capturing traffic and storing it efficiently in dump files, enabling easier packet analysis.

### Skills Learned

- Network Traffic Analysis: Monitoring and analyzing network traffic to identify suspicious patterns and security threats using tools like TCPDump and Wireshark, a critical skill for real-time threat detection in network security.
- Packet Capture and Analysis: Capture and analyze network packets to investigate and troubleshoot security incidents, vital for diagnosing network issues and identifying malicious activity.
- SSL/TLS Decryption: Decrypting SSL/TLS traffic using Wireshark, enabling the inspection of encrypted data and enhancing the ability to detect hidden threats in secure communications.
- Shell Scripting: Built proficiency in automating routine security tasks and creating custom logging tools through Bash shell scripting.
- Network Security: Strengthened foundational knowledge in securing networks by understanding various attack vectors and defense mechanisms, applying these principles in a simulated environment to mitigate potential risks.

### Tools Used

- TCPDump
- Wireshark
- Bash (Shell)

## Steps

![P1](https://github.com/user-attachments/assets/e0a24ac6-f342-4948-a6e6-f1c3045629ce)

Ref 1. Building the shell script for the logging tool and exploring target options.
- -i limits the interface to be captured, in this case, any interface is allowed
- The capture is limited to port 22
- -w writes the captured data to sshcatpure.pcap
- -C & -G set the size and time limits respectively.

![P2 Once the script is executed, the  pcap file becomes visible](https://github.com/user-attachments/assets/44b3f723-a42c-436a-a6e5-e22fbe68033d)

Ref 2. Once the script is executed, the .pcap file becomes visible.
- -x execute right is given to checkspy.sh
- dump file stopped at 3MB and creates a new file

![P4](https://github.com/user-attachments/assets/fa8ad694-01d7-45d5-9efd-7b2e33611d11)

Ref 3. The SSH traffic is easily noticeable on Wireshark. Though the source IP is from our host machine.
- After generating traffic, captured data is opened in Wireshark for readability.

![P5](https://github.com/user-attachments/assets/f9049d2c-ece8-47e0-8c53-0bb37160f7ee)

Ref 4. It is easier to locate packets using display filters.


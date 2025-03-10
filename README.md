## Objective
Gained hands-on experience in configuring networks, capturing traffic, and analyzing packets. Working with both Linux and Windows environments, I have set up network configurations, use tcpdump to capture traffic, and analyze packets with Wireshark.

## Skills Learned
- Network Configuration in Linux
- Network Configuration in Windows
- Traffic Capture with tcpdump
- Traffic Capture and Analysis with Wireshark

## Tools Used
- Linux Command Line (Terminal)
- Windows PowerShell
- tcpdump
- Wireshark

## Steps

### Part 1 - Network Configuration in Linux
1. Retrieve your Windows VM IP Address:
   - Launch Windows 10 virtual machine.
   - Run PowerShell as administrator.
   - Use `IPConfig` to get IPv4 address.
2. Launch Kali Linux virtual machine.
   - Open terminal: `Ctrl + Alt + T`.
   - Use `ip a` to view network information.
   - Open `/etc/hosts` file using `nano` or `vim`.
   - Edit the file to add `<IP_Address> winmachine`.
   - Test configuration by pinging `winmachine`.
   - Comment out the line in `/etc/hosts` and test again.

### Part 2 - Network Configuration on Windows
1. Access Windows PowerShell as an administrator.
   - Use `ncpa.cpl` to open network configuration.
   - View and note IPv4 settings.
   - Use `netsh` commands to set and reset DNS.

### Part 3 - Capturing Traffic with tcpdump
1. Open terminal on Linux machine.
2. Update and upgrade repository/package list.
3. Install tcpdump if not already installed.
4. Use `tcpdump -D` to list available adapters.
5. Capture traffic using tcpdump with various options and filters.
6. Save captured traffic to a file and read it using tcpdump.

### Part 4 - Capturing Traffic with Wireshark
1. Install Wireshark on Linux using terminal.
2. Launch Wireshark and capture traffic on `eth0` interface.
3. Stop and explore capture results.
4. Use display filters to analyze specific traffic.
5. Examine packet details and change views to understand different data presentations.

### Resources
- [Configuring Linux Network Interface File](https://www.devtutorial.io/how-to-manage-network-interfaces-on-ubuntu-server-22-04-ubuntu-server-22-04-p3097.html)
- [What is the /etc/hosts file](https://linuxhandbook.com/etc-hosts-file/)
- [Windows PowerShell netsh Command Explained](https://adamtheautomator.com/netsh/)
- [Basic Understanding of tcpdump](https://www.hugeserver.com/kb/install-use-tcpdump-capture-packets/)
- [Advanced tcpdump and Output Explained](https://opensource.com/article/18/10/introduction-tcpdump)
- [Tcpdump cheat sheet](https://www.comparitech.com/net-admin/tcpdump-cheat-sheet/)
- [Wireshark Installation on Linux](https://linuxtechlab.com/install-wireshark-linux-centosubuntu/)

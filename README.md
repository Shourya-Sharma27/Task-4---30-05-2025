# Task-4---30-05-2025
For this task, I explored basic firewall configuration using UFW (Uncomplicated Firewall) on Kali 
Linux. The goal was to understand how firewalls filter network traffic and how those rules are managed through simple commands.

I began by enabling UFW since it wasn’t active by default on my system. Once it was up and running, I checked the current 
firewall rules to see what was already allowed or blocked. After that, I added a rule to block port 23, which is commonly used for Telnet. 
Since Telnet is outdated and insecure, it made sense to use it as an example of something we'd want to block. To test whether the rule worked, 
I tried connecting to port 23 using the `telnet` command, and as expected, the connection was refused — confirming that the rule was doing its job.

Next, I allowed SSH traffic on port 22 because it's essential for remote access and I didn’t want to accidentally lock myself out. 
Once I was done testing the Telnet block, I deleted the rule for port 23 to bring things back to their original state. 
Throughout this process, I took note of the commands I used and captured screenshots of the firewall status, rules, and connection test results, 
which I’ve added in the `screenshots/` folder.

Doing this helped me see how a firewall actually works — not just in theory, but in practice. 
I now understand how controlling specific ports can reduce security risks and how UFW simplifies this process. 
This hands-on experience gave me a clearer picture of network traffic filtering and why these rules matter in real-world scenarios.

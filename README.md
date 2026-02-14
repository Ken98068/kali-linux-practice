# Kali-linux-practice



Notes, commands, and practice tools for learning Kali Linux and cybersecurity.
#Kali Linux Tools Notes

## 1. Nmap

* Used for network scanning and port discovery.
* Common commands:

  * `nmap 192.168.1.1` → basic scan of target IP.
  * `nmap -sV -p 1-100 192.168.1.1` → scan ports 1-100 with version detection.
* Flags:

  * `-sV` → detect service versions.
  * `-O` → detect operating system.
  * `-A` → aggressive scan (OS + version + scripts).

## 2. Netcat (nc)

* TCP/UDP connections, port listening, banner grabbing.
* Examples:

  * `nc -lvp 4444` → listen on port 4444.
  * `nc 192.168.1.5 80` → connect to port 80 of target.
* Useful for creating simple reverse shells or file transfers.

## 3. Burp Suite

* Web application testing and proxy tool.
* Intercepts HTTP requests and responses.
* Useful for:

  * Testing XSS, SQLi, CSRF vulnerabilities.
  * Replaying requests and modifying parameters.

## 4. Wireshark

* Network packet capture and analysis.
* Filters for analysis: `http`, `dns`, `tcp.port==80`.
* Learn to read packet headers, protocols, and data flow.

## 5. Key Tips

* Always use a controlled virtual lab environment.
* Take notes and practice commands regularly.
* Document every tool you experiment with for learning purposes.
* Combine tools for practical exercises (e.g., Nmap scan → Netcat connection → Burp testing).

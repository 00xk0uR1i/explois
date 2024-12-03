
# Ultimate Exploit 
![Capture](https://github.com/user-attachments/assets/5e645d72-868a-45f0-9ef5-8248650e1674)



## Description
`Ultimate Exploit ` is an advanced Bash script designed for ethical hackers and penetration testers. It automates the process of searching for vulnerable targets using Google dorks, testing for OWASP Top 10 vulnerabilities, and exploiting detected weaknesses. The script is tailored to simplify reconnaissance, vulnerability testing, and exploitation.

---

## Features
- **Automated Google Dork Search**: Utilizes dorks to find potential targets.
- **OWASP Top 10 Testing**:
  - SQL Injection (SQLi)
  - Cross-Site Scripting (XSS)
  - Local File Inclusion (LFI)
  - Cross-Site Request Forgery (CSRF)
  - Remote Command Execution (RCE)
  - Server-Side Request Forgery (SSRF)
  - Insecure Direct Object References (IDOR)
- **Exploitation Tools**:
  - Reverse shell generation and upload.
  - Automated database extraction with SQLMap.
  - Remote command execution.
- **Tool Management**: Automatically installs missing dependencies.
- **Netcat Listener**: Supports reverse shell handling.

---

## Requirements
- Linux system (Kali Linux recommended)
- Tools installed:
  - `curl`
  - `sqlmap`
  - `xsser`
  - `netcat`
  - `w3m`
  - `figlet`
  - `lolcat`
- Internet access.

The script will automatically install missing tools if not already present.

---

## Installation
1. Clone or download the script:
   ```bash
   git clone https://github.com/your-repo/ultimate-exploit-plus.git
   cd ultimate_exploits
   ```
2. Make the script executable:
   ```bash
   chmod +xultimate_exploits.sh
   ```

---

## Usage
1. **Run the script**:
   ```bash
   bash ultimate_exploits.sh
   ```

2. **Follow the prompts**:
   - Enter your **local IP (LHOST)** and **port (LPORT)** for reverse shell handling.

3. **Testing and Exploitation**:
   - The script will:
     - Perform reconnaissance using predefined Google dorks.
     - Test URLs for vulnerabilities.
     - Exploit identified weaknesses (e.g., SQLi, XSS, RCE).

4. **Start Listener** (for reverse shells):
   - Use `netcat` to listen for connections:
     ```bash
     nc -lvnp <LPORT>
     ```

---

## Example
```bash
bash ultimate_exploits.sh
```
- **Input**:
  - LHOST: `192.168.1.10`
  - LPORT: `4444`
- **Output**:
  - Vulnerable URLs.
  - Exploitation results (e.g., SQL dumped data, reverse shell access).

---

## Customization
- **Dorks**: Modify the dork list in the script to include your own search queries.
- **Tools**: Add or replace testing tools as needed.

---
## Proof of concept :





## Ethical Use
This script is intended for **authorized penetration testing** and **educational purposes only**. Unauthorized use is illegal and unethical. Always ensure you have permission to test and exploit a target.

---

## Contributors
- **Author**: k0ur1i  
- **Contributions**: Open for feature suggestions, enhancements, and bug fixes.  

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.  

---

## Disclaimer
Use this script responsibly. The author is not liable for any misuse or damage caused by the unauthorized use of this tool.

<a href="https://buymeacoffee.com/k0ur1i" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>


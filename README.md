# Phishing Simulation using StormBreaker 🚨

## Overview  
This project demonstrates a **phishing attack simulation** using **StormBreaker** to highlight cybersecurity risks, including unauthorized access to:  
- Camera  
- Location  
- Audio  
- Device details (IP, OS, Browser, etc.)  

The simulation aims to **raise awareness about social engineering threats** and educate users on protecting their digital privacy.

---

## Disclaimer
**This project is for educational and research purposes only. Unauthorized access to personal information is illegal and unethical. Use this simulation responsibly to raise awareness about cybersecurity threats.**

---

## Introduction
This project demonstrates a phishing attack simulation using **Storm Breaker** and **Ngrok**. The simulation highlights the risks of social engineering attacks that exploit camera access through malicious links.

---

## Prerequisites
Ensure you have the following installed:
- **Kali Linux or any Linux-based OS**
- **Git**
- **Python (for Ngrok setup)**
- **Ngrok** (to expose local server to the internet)
- **Storm Breaker** (for social engineering attack simulation)

---

## Installation & Setup
### Step 1: Clone the Storm Breaker Repository
```bash
cd /opt
git clone https://github.com/ultrasecurity/Storm-Breaker.git
```

⚠️ If the folder already exists, ensure it is empty before cloning.


### Step 2: Navigate to the Storm Breaker Directory
```bash
cd Storm-Breaker
```

### Step 3: Update System Packages**  
```bash
apt update
```

This ensures your system has the latest updates.

### Step 4: Install Dependencies**  
```bash
apt install python3-requests python3-colorama python3-psutil
```

### Step 5: Run the Installation Script**  
```bash
bash install.sh
```
If you encounter an error related to `requirements.txt`, open the file and ensure package names are correctly formatted.

---

### Step 6: Start the Tool
After installation, run the tool using: 
```bash
python3 storm-breaker.py
```
Follow on-screen instructions to generate phishing links and test the attack simulation.

### Step 7: Configure Ngrok for the Phishing Link**  
1. **Split the Terminal** to run Ngrok alongside StormBreaker.
2. **Add the Ngrok Authentication Token** (replace with your own token):  
   ```bash
   ngrok config add-authtoken YOUR_NGROK_AUTH_TOKEN
   ```
3. **Start Ngrok** with the following command:  
   ```bash
   ngrok http 2525
   ```

### Step 8: Generate and Share the Phishing Link
- Enter the **Ngrok URL** in Kali Linux browser.
- The tool will generate a **fake login page**.
- Share the phishing link with the target (for awareness purposes only!).

### Step 9: Capture Access
- Once the target clicks the link and grants permissions, Storm Breaker will access their information.
- The captured information will be stored in the local system.

---

## Troubleshooting  
- If `pip` is not working, try reinstalling it:
  ```bash
  apt install python3-pip --reinstall
  ```
- Ensure all dependencies in `requirements.txt` are correctly formatted.
- Run the script in a clean Python environment if issues persist.

---

## Prevention & Security Awareness
To protect against such attacks:
- **Do not click unknown links.**
- **Check URLs carefully before entering credentials.**
- **Use browser security features** to detect phishing pages.
- **Enable multi-factor authentication (MFA)** for accounts.

---

## Conclusion
This simulation helps in understanding social engineering attacks and how to defend against them. Ethical hackers and cybersecurity professionals can use this knowledge to educate users about online threats.

---

## License
This project is intended for **educational purposes only** and should not be used for illegal activities. Unauthorized use is strictly prohibited.

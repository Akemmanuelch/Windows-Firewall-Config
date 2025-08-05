# Windows-Firewall-Config
Configuring Windows Defender Firewall to allow FTP server access within a local network by enabling the firewall, creating inbound rules for port 21 (TCP), and verifying connectivity. Includes steps for securing and managing FTP access.

# Configuring Windows Defender Firewall for FTP Server Access

## 📌 Objective
This project demonstrates how to configure **Windows Defender Firewall** to allow FTP server connections within a local network.  
We will enable the firewall, open **TCP port 21**, and verify FTP connectivity between devices.

---

## 🛠️ Tools Used
- **Windows 10**
- **Windows Defender Firewall**
- **FileZilla Server**
- **Oracle VirtualBox**

---

## 🔹 Steps Taken

1. **Turn On Windows Defender Firewall**  
   - Opened **Windows Defender Firewall settings**.  
   - Enabled the firewall for **Private** and **Public** networks.  
   - *(Screenshot 1)*

2. **Create a New Inbound Rule**  
   - Opened **Windows Defender Firewall with Advanced Security**.  
   - Selected **New Rule → Port**.  
   - *(Screenshot 2)*

3. **Specify the Port and Protocol**  
   - Chose **TCP**.  
   - Set **Specific local ports** to **21** for FTP traffic.  
   - *(Screenshot 3)*

4. **Allow the Connection**  
   - Chose **Allow the connection** for the inbound FTP rule.  
   - *(Screenshot 4)*

5. **Apply Rule to All Profiles**  
   - Selected **Domain**, **Private**, and **Public** profiles.  
   - Named the rule **FTP Server**.  
   - *(Screenshot 5)*

6. **Verify FTP Rule**  
   - Checked that the **FTP Server** inbound rule was active and allowing connections.  
   - *(Screenshot 6)*

---

## 📷 Screenshots

1. ![Firewall Enabled](screenshots/firewall_enabled.jpeg)  
2. ![Inbound Rule - Select Port](screenshots/inbound_rule_port.jpeg)  
3. ![Inbound Rule - TCP Port 21](screenshots/tcp_port_21.jpeg)  
4. ![Inbound Rule - Allow Connection](screenshots/allow_connection.jpeg)  
5. ![Inbound Rule - Profiles](screenshots/inbound_rule_profiles.jpeg)  
6. ![Inbound Rule List](screenshots/inbound_rule_list.jpeg)  

---

## ✅ Outcome
- Successfully enabled **Windows Defender Firewall**.  
- Created and activated **inbound firewall rule** for FTP on **port 21**.  
- Verified that devices within the local network could connect to the FTP server.  

---

## 🔐 Security Note
While allowing port 21 enables FTP access, it is recommended to use **FTPS (FTP over TLS)** for secure file transfers to prevent credentials from being sent in plain text.

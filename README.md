## **Joining Linux and Windows Machines to Active Directory using Ansible**  

This Ansible project automates the process of joining **Ubuntu and Windows 11** machines to an **Active Directory (AD) domain**. While Windows supports domain joining natively, Linux requires multiple steps. This playbook simplifies and streamlines the process.  

---

### **🛠 Test Environment Setup**  
- **Configuration files:**  
  - `.ssh/config`  
  - `inventory.ini`  
  - `ansible.cfg` (Ensures `ansible_default_ipv4.address` works properly by preventing fact-gathering timeouts.)  

- **Windows Preparation:**  
  - Configured WinRM for Ansible control over Windows.  

---

### **📝 Playbook & Implementation**  
- **`playbook.yaml`** (Defines tasks for joining machines to AD.)  
- Customized the playbook for automation efficiency.  

---

### **🚀 Running the Playbook & Verification**  
- Successfully added:  
  - `Windows11_NewDeploy` → **sherwin.local domain**  
  - `TestServer` and `WebServer` → **sherwin.local domain**  
- Verified domain connection and machine status.  

---

This project ensures a seamless, automated approach to domain joining across both **Linux and Windows** environments using **Ansible**. 🚀

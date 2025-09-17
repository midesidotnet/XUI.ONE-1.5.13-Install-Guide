# XUI.ONE-1.5.13-Install-Guide
Step-by-step guide for installing XUI.ONE 1.5.13 on Ubuntu 20.04

Installing XUI.ONE 1.5.13 from scratch is simple if you follow this complete step-by-step tutorial. This guide assumes you have access to a dedicated server running Ubuntu 20.04.

---

## 💻 Recommended Server Specifications

To ensure a smooth IPTV experience with XUI.ONE, your server should meet these minimum specs:

* **CPU:** Intel Xeon or AMD Ryzen (6+ cores)
* **RAM:** 16–32 GB DDR4
* **Storage:** SSD or NVMe (480 GB or more)
* **Network:** Dedicated 1 Gbps port
* **Operating System:** Ubuntu 20.04 LTS (clean install)

---
## 🔧 Step 1: Get Root Access

Once your server is installed with Ubuntu 20.04, open your terminal and run:

```bash
sudo su -
```

Enter your server password when prompted. If successful, you will notice the terminal prompt change to `#`, indicating root access.

---

## 📦 Step 2: Install XUI.ONE

Run the following command to begin the installation process:

🔗 bash <(wget -qO- https://www.midesi.net/xuione/installxui.sh)

This installer will: 
* Display a welcome message 
* Download the xui-1.5.13.tar.gz archive 
* Extract all necessary files (install, database.sql, xui.tar.gz) 
* Automatically clean up the archive 
* Set execution permissions 
* Launch the installer script

---

## ⚙️ Step 3: Configuration Prompt

During installation, you will be asked:

```
Overwrite sysctl configuration? Recommended! (Y / N):
```

Type `y` and press Enter.

Installation will continue and finalize the setup, including your license.

---

## 🔐 Final Step: Panel Access Info

After a few moments, the script will output the following:

* ✅ Access URL to your XUI.ONE panel
* 🔑 Secret connection code
* 🗂️ MySQL credentials saved at: `/root/credentials.txt`

Please save this information securely, as it will be required to log in to your panel.

---

## 🚀 What’s Next: Setup and Configuration

Once your panel is installed, log in using the provided URL and credentials. You can now:

* Add your IPTV streams and channels
* Configure load balancers
* Set up EPG sources
* Add users and resellers
* Secure the panel using the built-in key regeneration tool


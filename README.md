>🛠️ **Support, Bug Reports & Feature Requests:** [Visit my GitHub Repository](https://github.com/dream-MT/M-IT-DCIM-Pro/discussions)

![M-IT DCIM PRO](https://imgur.com/3aYPhz2.png)

#  M-IT DCIM Pro
**The Future of Data Center Management. Built by an Admin, for Admins.**

## 📖 The Story: 20 Years of Data Center Experience
Over 20 years ago, my journey began as a DC Field Engineer. Back then, inventory meant endless Excel spreadsheets and hours of manually typing in MAC addresses and serial numbers. From Field Engineer to Senior DC Admin and finally Senior DC Manager, I've worked with the most professional enterprise solutions on the market. However, I always found they lacked crucial functions and day-to-day usability.

The result? After **7,000 hours of development** and over **50,000 lines of code**, *M-IT DCIM Pro* was born. A software that truly understands the daily grind of an admin and radically simplifies it.

> [!IMPORTANT]
> **Note on the Fast-Trial Version:** To guarantee a fast and smooth testing experience, I've excluded the 5+ GB AI databases from this trial version. This allows your test system to be up and running in under a minute!
> 
> Are you interested in experiencing the full power of our **100% offline AI** live in your data center? Feel free to reach out to me directly via the contact form inside the app.

---

## 📢 Latest Updates & New Features

### 📱 Mobile Ready & Tablet Workflow
M-IT DCIM Pro is now fully optimized for **mobile devices**. This enables seamless inventory management directly in front of the physical rack in the data center. 
* **Field-Inventory:** Use your tablet or smartphone to manage assets on the go.
* **Camera-Scan (AI Vision):** Use the integrated camera capture to scan hardware nameplates. The AI instantly extracts the serial number, model, and MAC address.
* **QR Code Tracking:** Every device generates a unique QR code. Print it, stick it on the server, and scan it with your tablet to instantly see its complete lifecycle and networking history!

### 🔄 Automatic Update Manager
The new M-IT DCIM update (v6.5.6) is here! I have integrated an automatic Update Manager directly into the web interface. From now on, you will be conveniently notified of new versions right in your dashboard! 
**To unlock this, please perform a manual update one last time:**
1. Open your `docker-compose.yml` and change the image version to `v6.5.6`.
2. Run `docker-compose pull` and `docker-compose up -d`.

---

## 🚀 Quick Start & Download

[⬇️ Download M-IT DCIM Quickstart Package (ZIP)](https://www.dropbox.com/scl/fi/hkj3yw38vrl20k40s5b53/m-it-dcim-pro-starter.rar?rlkey=eggy10xogy7u86fbf3ddrz76c&st=b2jkjzw2&dl=0)

## 📸 Visual Gallery

**Dashboard & Storage**
![M-IT DCIM PRO](https://i.imgur.com/rBpUhx2.png)

**Dashboard Slide right**
![M-IT DCIM PRO](https://i.imgur.com/J6QkAgv.png)

**2D Floorplan & Plan Upload**
![M-IT DCIM PRO](https://i.imgur.com/VopMeE7.png)

**Run the following from PowerShell (Clean Install):**
```powershell
docker-compose down -v
```
After that, use `M-IT_DCIM_START.bat` (or run `docker-compose up -d` from PowerShell).

**Default preconfigured credentials:**
* **User:** `admin`
* **Password:** `EnterprisePro123!`
---

## ⚙️ Enterprise Features

### 3D Digital Twin & Airflow Simulation
Forget static lists. Drag & drop your assets onto the 2D floor plan, and the system automatically generates an interactive 3D twin of your data center. Includes live airflow simulation and thermal heatmaps!

### Edge AI Copilot (100% Offline)
Integrated Artificial Intelligence (LLaMA3) that runs completely without cloud connections. Perfect for Critical Infrastructure (CRITIS) and highly secure environments.
* **Voice Control:** Voice-controlled provisioning of servers and VMs.
* **Predictive Maintenance:** The AI calculates thermal stress and warns you of hardware failures before they happen.
* **Vision Scanning:** Upload a photo of a hardware nameplate, and the AI handles the data extraction.

![M-IT DCIM 3D Twin](https://i.imgur.com/uQS4UkM.png)

### SPOF Analysis & Power Patching
Phase-safe power patching with live alerts. Simulate power outages at the push of a button (Blackout Test) and receive an instant PDF audit of all affected systems.

![M-IT DCIM 3D Twin](https://i.imgur.com/2PBX305.png)

### SCADA & Industrial Protocol Engine
Native support for Modbus TCP, BACnet/IP, and SNMP. Integrate CRAC units, UPS systems, and Smart PDUs directly into your live visualization.

![M-IT DCIM Trace](https://i.imgur.com/aMjyBby.png)

---

**Setup**
![M-IT DCIM Local KI-Engine](https://i.imgur.com/D2Za3a5.png)

**Thermalmap**
![M-IT DCIM Local KI-Engine](https://i.imgur.com/LgW5R1k.png)

**Spacemap**
![M-IT DCIM Local KI-Engine](https://i.imgur.com/5tJcBLI.png)

**3D-Edit Mode**
![M-IT DCIM Local KI-Engine](https://i.imgur.com/MMuOYXf.png)

**Hardware Settings**
![M-IT DCIM Hardware Settings](https://i.imgur.com/2KTrrbQ.png)

**Virtual Machines Management (ProxMox / VCenter Connect)**
![M-IT DCIM Hardware Settings](https://i.imgur.com/3dbYjiH.png)

---

## 🛠️ Installation (Docker Native)
Time is money. Deployment takes less than 1 minute.

This image is the sealed core engine. To run it, you need the official customer release package (`M-IT_DCIM_START.bat` and `docker-compose.yml`), which automatically orchestrates the AI sidecars and databases.

```text
========================================================================
🚀 M-IT DCIM PRO - QUICK START GUIDE
========================================================================
"The Future of Data Center Management. Built by an Admin, for Admins."

Welcome to M-IT DCIM Pro! This package contains the deployment 
files (Docker Compose) required to run the DCIM safely and isolated on 
your local machine or server.

------------------------------------------------------------------------
⚠️ PREREQUISITES
------------------------------------------------------------------------
Before you begin, ensure your system meets the following requirements:
1. Docker Engine or Docker Desktop must be INSTALLED and RUNNING.
2. An active internet connection (Only required for the initial 
   download of the secure Docker images and the offline AI model).

------------------------------------------------------------------------
🛠️ INSTALLATION & STARTUP
------------------------------------------------------------------------

STEP 1: EXTRACT THE PACKAGE
Extract this ZIP file to a permanent location on your server or PC 
(e.g., C:\MIT_DCIM or /opt/mit_dcim).

STEP 2: START THE INFRASTRUCTURE
We have fully automated the deployment process.

► For Windows Users:
  Simply double-click the included batch file:
  [ M-IT_DCIM_START.bat ]

► For Linux / macOS / Terminal Users:
  Open your command line, navigate to this folder, and run:
  docker-compose up -d

STEP 3: INITIALIZATION (First Run Only)
The system will now securely download the Core Engine, the PostgreSQL 
Database, and the local Edge-AI container. Depending on your internet 
speed, this may take a few minutes. 
(Note: The local AI Model is >5 GB to ensure 100% offline data privacy).

------------------------------------------------------------------------
🌐 ACCESSING THE DASHBOARD
------------------------------------------------------------------------
Once the terminal indicates that the containers are "Started" or "Up", 
open your modern web browser (Chrome, Edge, Firefox, Safari) and go to:

👉 http://localhost:5000
(If installed on a remote server, replace 'localhost' with the Server IP)

------------------------------------------------------------------------
🔑 ACTIVATING YOUR LICENSE
------------------------------------------------------------------------
To unlock the Enterprise Features (3D Digital Twin, Offline LLaMA3 AI, 
SPOF Power Analysis), you require a valid RSA License Token.

1. Open the application in your browser.
2. You will be greeted by the licensing screen.
3. Paste the Token string provided by our sales team into the field.
4. Click Activate. The system will verify the cryptographic signature 
   offline and unlock your portal.

------------------------------------------------------------------------
🛑 STOPPING / RESTARTING THE SYSTEM
------------------------------------------------------------------------
To safely shut down the DCIM and all connected databases without data loss,
open your terminal in this directory and run:
docker-compose down

To update the system in the future, simply run:
docker-compose pull
docker-compose up -d

------------------------------------------------------------------------
🔑 YOUR TRIAL LICENSE
------------------------------------------------------------------------
P.S.: Did you know? > You can now test the exclusive PRO and ENTERPRISE 
features (like the AI Copilot (requires downloading the Ollama Package), 
3D Rack View, Audit-Log, and smart connections to CRAC Units, PowerStations, 
IoT, and Zigbee) completely free for 15 days in your own environment!

Simply click on any PRO feature in your dashboard to request an upgrade, 
or reply directly to this email. I'll send you your trial license key immediately!

========================================================================

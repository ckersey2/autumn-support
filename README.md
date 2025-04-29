# 🛠️ Windows Update Diagnostic Script for Windows 11

This script helps check and troubleshoot why Windows 11 is **not automatically checking for or installing updates**.

---

## 📦 What This Script Does

- Checks if key Windows Update services are running  
- Looks for any Group Policy or Registry settings that block updates  
- Lists recent update history  
- Checks scheduled tasks related to updates  
- Tries to detect if updates are available

---

## 🧰 What You'll Need

- A **Windows 11** PC  
- **Administrator access** (you can approve changes when asked)  
- An **internet connection**

---

## 👣 Step-by-Step Instructions

### 1. **Download the Script**

- Go to this page: [🔗 *Windows 11 Update Debug Script*](https://gist.github.com/ckersey2/155079695b567c4c0fa642bafdbaf21e#file-check-windowsupdate-ps1)
- Click the **“Raw”** button  
- Right-click the page and choose **“Save As...”**  
- Save it to your **Desktop** as `Check-WindowsUpdate.ps1`

---

### 2. **Open PowerShell as Administrator**

- Click the **Start** menu  
- Type `powershell`  
- Right-click **Windows PowerShell**  
- Choose **“Run as administrator”**  
- Click **Yes** if a message asks for permission

---

### 3. **Run the Script**

In the PowerShell window, run these commands one by one (each line is a separate command):

```powershell
cd $HOME\Desktop
Set-ExecutionPolicy RemoteSigned -Scope Process
.\Check-WindowsUpdate.ps1
```

- If asked to confirm, type Y and press Enter
- Let the script run—it may take a few minutes

## 🧾 What to Expect
- You'll see messages showing what the script is checking
- It does not change any settings, it only checks and shows results
- When it’s done, you’ll see: ✅ Diagnostic complete.

## 🆘 If You Need Help
If the script shows red or yellow warnings, or you're still not getting updates:
- Take a screenshot of the PowerShell window
- Send it for me to review

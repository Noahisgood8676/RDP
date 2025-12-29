# 🚀 FREE-RDP-MADE-BY-XERO-USING-BORE

A high-performance Windows Remote Desktop (RDP) solution running on GitHub Actions. This project features an **Auto-Restart loop** (runs forever) and a **Persistent Data System** to keep your files safe between sessions.

---

## 🌟 Key Features
* **100% Free:** No tokens or accounts required.
* **Security Bypass:** Automatically generates strong credentials to meet Windows complexity policies.
* **Persistent Storage:** Files in `C:\Users\runneradmin\Desktop\SavedData` are backed up and restored automatically.
* **Auto-Restart:** Triggers a new session every 6 hours to bypass GitHub limits.
* **Fast Connection:** Powered by [Bore](https://github.com/ekzhang/bore) for low-latency TCP tunneling.

---

## 🛠️ Setup Instructions

### 1. Start the Machine
1.  Go to the **Actions** tab in this repository.
2.  Select the workflow: `FREE-RDP-MADE-BY-XERO-USING-BORE`.
3.  Click **Run workflow** > **Run workflow**.

### 2. Get your Credentials & Port
1.  Click on the active workflow run.
2.  **For User/Pass:** Open the **🛠️ Setup Windows (XERO-Edition)** step. Look for the **USERNAME** and **PASSWORD** generated for that session.
3.  **For Port:** Open the **🚀 Launch Bore Tunnel** step. Look for the line: `listening at bore.pub:XXXXX`.

### 3. Connect via RDP
1.  Open **Remote Desktop Connection** on your PC.
2.  **Computer:** `bore.pub:XXXXX` (Use the port from step 2).
3.  **Username:** (Use the random username from step 2).
4.  **Password:** (Use the random password from step 2).

---

## 💾 How the Save System Works (IMPORTANT)

GitHub wipes the machine every 6 hours. To keep your files:
1.  Open the folder **`SavedData`** on the Desktop of the RDP.
2.  **Move all files you want to keep into this folder.**
3.  When the session ends (or if you cancel it), the system will upload this folder.
4.  When the next session starts, your files will be restored automatically.

> [!WARNING]  
> Any files saved outside of `C:\Users\runneradmin\Desktop\SavedData` will be **deleted forever** when the session restarts.

---

## 👤 Credits
**Created by:** XERO  
**Tooling:** Powered by [Bore](https://github.com/ekzhang/bore) and GitHub Actions.

---

## ⚖️ Disclaimer
This project is for educational and testing purposes only. Usage of GitHub Actions for RDP must comply with [GitHub's Terms of Service](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service).

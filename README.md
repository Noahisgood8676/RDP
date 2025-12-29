# 🚀 FREE-RDP-MADE-BY-XERO-USING-BORE

A high-performance Windows Remote Desktop (RDP) solution running on GitHub Actions. This project features an **Auto-Restart loop** (runs forever) and a **Persistent Data System** to keep your files safe between sessions.

---

## 🌟 Key Features
* **100% Free**
* **Persistent Storage:** Files saved in the `C:\Users\runneradmin\Desktop\SavedData` folder are automatically backed up and restored.
* **Auto-Restart:** Automatically triggers a new session every 6 hours to bypass GitHub limits.
* **Fast Connection:** Uses **Bore** (TCP Tunneling) for low-latency mouse and keyboard input.

---

## 🛠️ Setup Instructions

### 1. Start the Machine
1.  Go to the **Actions** tab in this repository.
2.  Select the workflow: `FREE-RDP-MADE-BY-XERO-USING-BORE`.
3.  Click **Run workflow** > **Run workflow**.

### 2. Get your Connection Address
1.  Click on the active workflow run.
2.  Open the **🚀 Launch Bore Tunnel** step.
3.  Look for the line: `listening at bore.pub:XXXXX`.
4.  Copy that address (e.g., `bore.pub:12345`).

### 3. Connect via RDP
1.  Open **Remote Desktop Connection** on your PC.
2.  **Computer:** Paste the address from the logs (e.g., `bore.pub:12345`).
3.  **Username:** `SkibidiXero`
4.  **Password:** `SkibidiXeroisHot`

---

## 💾 How the Save System Works (IMPORTANT)

GitHub wipes the machine every 6 hours. To keep your files:
1.  Paste this into the file explorer path box **`C:\Users\runneradmin\Desktop\SavedData`** on the FREE-RDP made by XERO.
2.  **Move all files you want to keep into this folder.**
3.  When the session ends (or if you cancel it), the system will upload this folder.
4.  When the next session starts, your files will be waiting for you in that same folder.

> [!WARNING]  
> Any files saved outside of `C:\Users\runneradmin\Desktop\SavedData` will be **deleted forever** when the session restarts.

---

## 👤 Credits
**Created by:** XERO  
**Tooling:** Powered by [Bore](https://github.com/ekzhang/bore) and GitHub Actions.

---

## ⚖️ Disclaimer
This project is for educational and testing purposes only. Usage of GitHub Actions for RDP must comply with [GitHub's Terms of Service](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service).


# 📦 Incantation - UnderGround SMTP Checker

Welcome to **Incantation.exe** — a lightweight, encrypted SMTP checker built for speed, reliability, and privacy. This tool helps you verify if SMTP credentials are valid, logs the results, and ensures access is protected via a license system.

---

## 🚀 How to Use

### 1️⃣ Prepare Your SMTP List

- Create a text file named: `smtps.txt`
- Place it in the same folder as `incantation.exe`
- Add your SMTPs in this format **(one per line)**:

```

smtp.example.com:587|[user@example.com](mailto:user@example.com)|password123
smtp.gmail.com:465|[example@gmail.com](mailto:example@gmail.com)|app-password
smtp.mail.com:587||api-key-or-token

````

> Use the correct format:  
> `host:port|username|password`

---

### 2️⃣ Run the Program

1. **Double-click** `incantation.exe`  
   or  
   **Run from Command Prompt**:
   ```cmd
   incantation.exe


2. On first run, you will be asked to **enter your license key**:

   ```
   🔐 Enter your license key:
   ```

3. Once verified, the tool will remember your license and won't ask again on future runs (unless the license is invalidated or moved to another PC).

---

### 3️⃣ What Happens Next

* It will begin checking your SMTP credentials.
* You'll see either ✅ (valid) or ❌ (invalid) next to each line.
* It saves **only valid** SMTPs to:

  ```
  valid_smtps.txt
  ```

---

## 🔐 License Protection

* This app uses a license system to protect against abuse.
* Your key is verified with the license server on first use.
* After successful activation, your device is **unlocked permanently** unless revoked or moved.
* License data is securely encrypted in:

  ```
  .underground_license
  ```

---

## 🗂 Files You’ll See

| File                   | Purpose                            |
| ---------------------- | ---------------------------------- |
| `incantation.exe`      | The main executable                |
| `smtps.txt`            | Your SMTP credentials (input)      |
| `valid_smtps.txt`      | Generated: stores only valid SMTPs |
| `.underground_license` | Encrypted license key cache        |

---

## ⚠️ Notes

* Make sure you are **connected to the internet** when running for the first time (to verify license).
* Your SMTPs must support **PLAIN SMTP Authentication**.
* Gmail accounts require **App Passwords**, not your real Gmail password.
* This tool does **not send emails**, it only **checks** if SMTP credentials are valid.

---

## ❓ Troubleshooting

* **Nothing happens?**
  Run via Command Prompt to see output:

  ```cmd
  incantation.exe
  ```

* **License error?**
  Make sure you're entering a correct license and you're connected to the internet.

* **All SMTPs show ❌?**
  Check that:

  * Ports are correct (usually `587` or `465`)
  * You used app passwords or valid credentials
  * There is no firewall blocking the app

---

## 📬 Support

* Get help or report issues here:
  [https://github.com/consolesoft/incantation](https://github.com/consolesoft/incantation)
* Or contact: `support@yourdomain.com`

---

## 💻 Example Output

```
🔐 Enter your license key:
✅ License confirmed and device unlocked.

📬 Checking SMTP credentials...
✅ smtp.gmail.com:465|me@gmail.com|myapppass
❌ smtp.fake.com:587|user@bad.com|wrongpass

✅ Done. Valid SMTPs saved to valid_smtps.txt
```

---

## 🔥 Credits

Made with love by **gameThe0ry**
License server by **UnderGr0und**

```

---


- Telagram @gamethe0ry

```

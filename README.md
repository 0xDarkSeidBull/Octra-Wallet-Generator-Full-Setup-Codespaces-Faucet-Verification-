###  Octra Test Network (Public)

![ChatGPT Image Jun 30, 2025, 08_15_56 AM](https://github.com/user-attachments/assets/903777d1-c3ba-4cb5-ad45-a077053114c8)

---

## Requirements

Linux/Ubuntu OS

* **Linux/Ubuntu** – Native support, recommended.
* **VPS** – Any Ubuntu-based server works great.
* **Windows** – Use WSL to run Ubuntu by following this [guide](https://learn.microsoft.com/en-us/windows/wsl/install).
* **Codespace** – No VPS? Use [GitHub Codespace](https://github.com/features/codespaces), create a blank template and run your codes instantly.

---

### 1: Create Codespace

Go to https://github.com/octra-labs/wallet-gen

Click <> Code > Create codespace on main

### 2.  Install Bun

```bash
curl -fsSL https://bun.sh/install | bash
````

Restart the shell:

```bash
exec $SHELL
```

Check version:

```bash
bun --version
```

---

### 3.  Open Port 8888 (optional if testing locally)

```bash
sudo apt update && sudo apt install ufw -y
sudo ufw allow 8888
```

---

### 4.  Clone the Wallet Generator

```bash
git clone https://github.com/octra-labs/wallet-gen
cd wallet-gen
```

---

### 5.  Install Dependencies

```bash
bun install
```

---

### 6. 🔧 Build the Executable (Optional)

```bash
bun run build
```

This creates a `wallet-generator` binary.

---

### 7.  Start the Wallet Generator

```bash
bun start
```

> Access the UI at:
> 🔗 **[http://localhost:8888](http://localhost:8888)** (Codespace browser will expose this link)

---

## Claim Faucet Tokens

Once a wallet is generated, copy your **Octra address** and visit:

🔗 [https://faucet.octra.network](https://faucet.octra.network)

Paste the address to claim test tokens.

---

## Verify on the Octra Explorer

Use your transaction hash to view and verify on:

🔍 [https://explorer.octra.network](https://explorer.octra.network)

## TASK 1: Execute Transactions

## 1. Install Python & Git
```
sudo apt update
sudo apt install python3 python3-pip python3-venv python3-dev git -y
```

## 2. Clone the Octra Pre Client Repository
```
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client
```
## 3. Set Up Python Virtual Environment
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
## 4. Configure Your Wallet
```
cp wallet.json.example wallet.json
nano wallet.json
```
## Replace the contents with your wallet info:
 Replace the Following in wallet.json:
 
"priv": Paste your private key in Base64 format (not raw hex)

"addr": Paste your Octra wallet address, which starts with oct...
Press Ctrl + X, then Y, then Enter to save and exit the file.

## 5. Start the Octra CLI
```
source venv/bin/activate
python3 cli.py
```
If everything is correct, you’ll see an interactive CLI menu.
![image](https://github.com/user-attachments/assets/c7b72c46-0d7c-4f81-a4e9-d42a149c1af7)

## 6. Send Transactions
Send transactions to my address: octG624SYptsXJfmu1A4FQmQyJ2N1PV8BDmt3Bs1wyYbDNj

Use [Octra Explorer](https://octrascan.io/) to find more Octra addresses.

---
## Join the Community
Have questions or want to participate?

🔗 Join the Octra Discord: https://discord.gg/octra
Get support, share feedback, and connect with the community!
##  Tips

* Always keep your mnemonic/private key secure.
* If you want to run the UI publicly, launch the server on `0.0.0.0` instead of `localhost`:

```bash
bun start --host 0.0.0.0
```

---

##  Security Warning

⚠️ This tool generates **real cryptographic wallets**. Do **NOT** use it on shared or insecure environments for mainnet/private keys.

---





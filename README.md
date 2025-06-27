### 🚀 Octra Wallet Generator – Codespaces Full Guide


  ✅ Requirements:
  GitHub account

  Codespaces access

  Octra Wallet Generator GitHub




### 1: Create Codespace

Go to https://github.com/octra-labs/wallet-gen

Click <> Code > Create codespace on main

### 2. 📥 Install Bun

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

### 3. 🔓 Open Port 8888 (optional if testing locally)

```bash
sudo apt update && sudo apt install ufw -y
sudo ufw allow 8888
```

---

### 4. 🧠 Clone the Wallet Generator

```bash
git clone https://github.com/octra-labs/wallet-gen
cd wallet-gen
```

---

### 5. 📦 Install Dependencies

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

### 7. 🚀 Start the Wallet Generator

```bash
bun start
```

> Access the UI at:
> 🔗 **[http://localhost:8888](http://localhost:8888)** (Codespace browser will expose this link)

---

## 💸 Claim Faucet Tokens

Once a wallet is generated, copy your **Octra address** and visit:

🔗 [https://faucet.octra.network](https://faucet.octra.network)

Paste the address to claim test tokens.

---

## 🧾 Verify on the Octra Explorer

Use your transaction hash to view and verify on:

🔍 [https://explorer.octra.network](https://explorer.octra.network)

---

## 📌 Tips

* Always keep your mnemonic/private key secure.
* If you want to run the UI publicly, launch the server on `0.0.0.0` instead of `localhost`:

```bash
bun start --host 0.0.0.0
```

---

## 🔐 Security Warning

⚠️ This tool generates **real cryptographic wallets**. Do **NOT** use it on shared or insecure environments for mainnet/private keys.

---


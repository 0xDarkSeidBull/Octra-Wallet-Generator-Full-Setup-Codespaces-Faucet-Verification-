# 🦾 Octra Wallet Generator – Full Setup Guide (Codespaces + Faucet + Verification)

This guide walks you through running the [Octra Wallet Generator](https://github.com/octra-labs/wallet-gen) using GitHub Codespaces. It includes generating wallets, claiming faucet tokens, and verifying transactions on the Octra blockchain.

---

## 🚀 What You'll Do

✅ Generate secure Octra wallets  
✅ Use faucet to get test tokens  
✅ Run everything inside GitHub Codespaces  
✅ Verify your transaction on the Octra explorer

---

## 🧱 Prerequisites

- ✅ GitHub account
- ✅ Codespaces access (comes with GitHub free or pro)
- ✅ Basic terminal knowledge (copy-paste works!)

---

## ⚙️ Step 1: Open Codespace

1. Visit: [https://github.com/octra-labs/wallet-gen](https://github.com/octra-labs/wallet-gen)
2. Click the green `Code` button → **"Create codespace on main"**

---

## 💻 Step 2: Install Bun

Inside the Codespaces terminal:

```bash
curl -fsSL https://bun.sh/install | bash
exec $SHELL
bun --version

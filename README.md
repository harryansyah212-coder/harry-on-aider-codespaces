# 🤖 HARRY ON — Aider Integration for GitHub Codespaces

**One-click setup!** Buka di GitHub Codespaces, semua ter-install otomatis.

---

## 🚀 Quick Start (30 Detik)

### 1. Klik "Open in GitHub Codespaces"

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/harryon/aider-codespaces)

### 2. Tunggu Setup Otomatis (2-3 menit)

Terminal akan menampilkan:
```
🤖 HARRY ON — GitHub Codespaces Auto-Setup
[1/6] Installing Aider...
[2/6] Installing tools...
[3/6] Setting up HARRY ON...
...
🎉 HARRY ON Aider Setup COMPLETE!
```

### 3. Isi API Keys (Sekali saja)

```bash
cp ~/.harry-on/.env.template ~/.harry-on/.env
nano ~/.harry-on/.env
```

Isi dengan API keys:
```
OPENAI_API_KEY=sk-your-key
ANTHROPIC_API_KEY=sk-ant-your-key
MOONSHOT_API_KEY=sk-your-key
```

### 4. Mulai Coding!

```bash
# Buat project baru
harry-start my-ecommerce web

# Masuk ke folder
cd my-ecommerce

# Jalankan Aider dengan AI rotation
harry-aider
```

---

## 📚 Commands

| Command | Fungsi |
|---------|--------|
| `harry-aider` | Launch Aider dengan auto AI rotation |
| `harry-start <name> [type]` | Buat project baru |
| `harry-resume` | Resume dari checkpoint terakhir |
| `harry-status` | Cek status HARRY ON |

---

## 🤖 AI Rotation

Jika satu AI busy, otomatis pindah ke AI berikutnya:

1. **GPT-5.5 Pro** (50%) — Primary coding
2. **Claude Opus 4.8** (30%) — Creative & analysis
3. **Kimi K2.6** (20%) — Indonesian & long docs
4. **Gemini 1.5 Pro** (0%) — Emergency backup

---

## 🎯 Features

- ✅ Auto-install Aider + dependencies
- ✅ Multi-AI auto-rotation
- ✅ Git checkpointing otomatis
- ✅ Resume dari checkpoint
- ✅ VS Code extensions pre-installed
- ✅ Prettier + ESLint + Tailwind ready
- ✅ Node.js + Python ready

---

## 🛡️ Anti-Busy Mechanism

```
🤖 Attempt 1/5
🎯 AI: GPT-5.5 Pro
⚠️ GPT-5.5 Pro busy
🔄 Switching to Claude Opus 4.8...
🤖 Attempt 2/5
🎯 AI: Claude Opus 4.8
✅ Success!
```

---

## 📁 Project Structure

```
📦 aider-codespaces
├── .devcontainer/
│   └── devcontainer.json      # Codespaces config
├── .github/
│   └── workflows/
│       └── setup.yml          # CI/CD (optional)
├── harry-on-setup.sh          # Auto-setup script
├── harry-aider-integration.py # Python module
└── README.md                  # This file
```

---

## 🔧 Manual Setup (Jika Tidak Pakai Codespaces)

```bash
# Clone repo
git clone https://github.com/harryon/aider-codespaces.git
cd aider-codespaces

# Jalankan setup
bash harry-on-setup.sh

# Isi API keys
source ~/.bashrc
```

---

## 📝 License

MIT License — HARRY ON V1 MVA UNLIMITED v2.0.0

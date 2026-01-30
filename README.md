# 🔗 Generate Shortlink System
Sistem pemendek link dengan subdomain random + path random untuk keperluan CPA/Affiliate marketing.

## 📱 Cara Deploy dari Android

### Opsi 1: Deploy via Termux (Recommended)
```bash
# Install Termux dari F-Droid, lalu:
pkg update && pkg upgrade -y
pkg install nodejs git -y
npm install -g wrangler

# Clone repo Anda
git clone https://github.com/username/generate-shorlink.git
cd generate-shorlink

# Setup Wrangler
wrangler login
wrangler kv:namespace create "LINKS_DB"
# Copy ID KV ke wrangler.toml

# Deploy
wrangler deploy

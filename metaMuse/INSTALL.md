# Meta Muse CLI (Muse Code) - Install Guide

## 1. Requirements
- macOS / Linux, arm64 or x86_64
- Windows: use WSL2 (no native build)
- Needs: `curl`, `bash`, Meta account
- Installs to: `~/.local/bin/muse`

## 2. Install
```bash
curl -fsSL https://dev.meta.ai/install.sh | bash
```

Safer (audit first):
```bash
curl -fsSL https://dev.meta.ai/install.sh -o install.sh
less install.sh
bash install.sh
```

Custom location / no PATH edit:
```bash
MUSE_NO_MODIFY_PATH=1 MUSE_INSTALL_DIR="$HOME/bin" bash install.sh
```

## 3. Verify + Start
```bash
exec $SHELL -l
which muse
muse --version
muse  # first run: browser OAuth sign-in / muse login
```

## 4. Subscription charges (Muse, Sept 8 2026, US-only 18+)
- Free: $0 with usage limit (payment card required on file)
- Power: $20/month - 500M Muse tokens/week
- Maximum: $100/month - 3B Muse tokens/week
- Auto-renews monthly. Most users stay on Free per Meta.

Access: muse.ai, iOS/Android, WhatsApp, CLI uses same Meta account.
Docs: https://dev.meta.ai/docs/muse-code

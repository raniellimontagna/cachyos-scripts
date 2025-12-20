# CachyOS Scripts

A collection of useful scripts for CachyOS and general Linux system management.

## 📁 Project Structure

### Monitor Scripts (`monitor-scripts/`)

Scripts for managing monitor configurations using KDE's kscreen-doctor utility.

- **`work-mode.sh`** - Work Mode Configuration

  - Sets DP-1 as primary monitor with normal rotation
  - Sets DP-2 with right rotation (90° clockwise) for vertical content (code, documents, chat)
  - Positions DP-2 at coordinates (1920, 0)
  - Ideal for productivity work with vertical monitor setup

- **`racing-mode.sh`** - Racing/Gaming Mode Configuration
  - Sets DP-2 as primary monitor with normal rotation
  - Sets DP-1 with normal rotation
  - Positions DP-2 at coordinates (1920, 0)
  - Perfect for racing games with steering wheel or gaming sessions requiring both monitors in landscape

## 🚀 Usage

### Monitor Scripts

Make the scripts executable and run them:

```bash
chmod +x monitor-scripts/*.sh
./monitor-scripts/work-mode.sh
# or
./monitor-scripts/racing-mode.sh
```

#### Setting up Keyboard Shortcuts in KDE

To quickly switch between monitor profiles using keyboard shortcuts:

1. Open **System Settings** → **Shortcuts** → **Custom Shortcuts**
2. Click **Edit** → **New** → **Global Shortcut** → **Command/URL**
3. In the **Trigger** tab, set your desired keyboard shortcut (e.g., `Meta+F1` for work mode)
4. In the **Action** tab, enter the full path to the script:
   ```
   /home/ranni/www/personal/cachyos-scripts/monitor-scripts/work-mode.sh
   ```
5. Click **Apply**
6. Repeat steps 2-5 for the racing mode with a different shortcut (e.g., `Meta+F2`)

**Suggested shortcuts:**

- `Meta+F1` → Work Mode
- `Meta+F2` → Racing Mode

## 📝 Requirements

- **KDE Plasma** desktop environment
- **kscreen-doctor** utility (part of KDE Plasma)

## 🤝 Contributing

Feel free to add more useful scripts to this repository. Please maintain the organized folder structure and update this README accordingly.

## 📄 License

These scripts are provided as-is for personal use.

# wireguard-access-manager
Fine-grained client access control and IP segmentation for maximum wireguard VPN security.
![WireGuard Manager Main Menu](assets/1.png)
# 📦 Installation

WireGuard Access Manager provides a secure and user-isolated VPN configuration tool for Linux systems.

---
## Key Features:

- Secure and user-isolated VPN configurations
- Fine-grained client access control
- IP segmentation for enhanced security
- Easy installation with a single command


## ✅ Quick Install (Recommended)

You can install the WireGuard Manager globally with one command:

```bash
curl -sfL https://raw.githubusercontent.com/nazmul-islam21/wireguard-access-manager/main/wg-nstall.sh | sh -s
```

This will:

- Install required packages (`wireguard-tools`, `qrencode`, `zip`, `unzip`, etc.)
- Download the `wireguard_manager` script
- Place it in `/usr/local/bin/` as a global command
- Make it executable

After installation, you can run the manager from anywhere using:

```bash
wireguard_manager
```
## Screen Short

![WireGuard Manager Main Menu](assets/1.png)
![WireGuard Manager Main Menu](assets/2.png)
![WireGuard Manager Main Menu](assets/3.png)
![WireGuard Manager Main Menu](assets/4.png)
![WireGuard Manager Main Menu](assets/5.png)
---

## 🧱 Requirements

| Component          | Required                                     |
|--------------------|----------------------------------------------|
| Linux OS           | ✅ Ubuntu, Debian, Rocky, AlmaLinux           |
| Bash Shell         | ✅ `/bin/bash`                               |
| WireGuard          | ✅ `wireguard-tools`                         |
| QR Code Generator  | ✅ `qrencode`                                |
| Archiver Tools     | ✅ `zip`, `unzip`                            |
| Internet Access    | ✅ Required to fetch installer and dependencies |

---

## 🖥️ Supported Distributions

- ✅ Ubuntu 20.04 / 22.04 / 24.04
- ✅ Debian 10 / 11 / 12
- ✅ Rocky Linux 8 / 9
- ✅ AlmaLinux 8 / 9
- ✅ Other bash-based Linux systems (manual setup supported)

---

## 🔒 File Locations After Install

| Path                                | Purpose                          |
|-------------------------------------|----------------------------------|
| `/usr/local/bin/wireguard_manager`  | The main executable script       |
| `~/.wireguard_manager/configs/`     | Client configuration files       |
| `~/.wireguard_manager/iptables/`    | IPTables per-client rule scripts |
| `~/.wireguard_manager/qrcodes/`     | QR code PNG files                |
| `~/wg-backup/`                      | Backup zip files                 |

---

## 🧪 Post-Install Test

After installation, verify the command:

```bash
wireguard_manager
```



You should see the WireGuard Access Manager main menu.

---

## 💡 How to Update

To update the tool manually later:

```bash
sudo rm -f /usr/local/bin/wireguard_manager
curl -sfL https://raw.githubusercontent.com/nazmul-islam21/wireguard-access-manager/main/wireguard_manager.sh -o /usr/local/bin/wireguard_manager
sudo chmod +x /usr/local/bin/wireguard_manager
```

---

## 🛠 Uninstall

To completely remove WireGuard Manager:

```bash
sudo rm -f /usr/local/bin/wireguard_manager
rm -rf ~/.wireguard_manager ~/wg-backup
```

---

# 🚀 You're now ready to securely manage WireGuard with per-client access control!

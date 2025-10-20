# 🕊️ PigeonHole Package Repository

Welcome to the PigeonHole package repository.   

This repository provides access to our latest APT, YUM and Chocolatey packages for seamless installation and updates of PigeonHole across your systems.

# 📦 About This Repository

This repo is designed to make it simple to:
Install PigeonHole to your Debian, Ubuntu, RHEL, CentOS, AlmaLinux, Rocky Linux or Windows systems.

Stay up to date with the latest CLI tools, security updates, and performance improvements.


# 💡 Getting Started

You can add this repository to your system using your package manager:
## Debian / Ubuntu:
```
curl -fsSL https://packages.pigeono.io/gpg.pub | sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/pigeono.gpg
echo "deb [arch=amd64] https://packages.pigeono.io/apt noble main" | sudo tee /etc/apt/sources.list.d/pigeono.list
sudo apt update && sudo apt install pigeonhole-cli
```


## RHEL / CentOS / AlmaLinux / Rocky:
```
sudo rpm --import https://packages.pigeono.io/gpg.asc
sudo tee /etc/yum.repos.d/pigeonhole.repo <<EOF
[pigeonhole]
name=PigeonHole Repository
baseurl=https://packages.pigeono.io/rpm/
enabled=1
gpgcheck=1
gpgkey=https://packages.pigeono.io/gpg.asc
EOF
sudo dnf install -y pigeonhole-cli
```

# 🧭 Learn More

To learn more about PigeonHole, the mission, and how we're building the secure, end-to-end file transfer tool for teams and individuals, visit the official site:

👉 [https://pigeono.io/](https://pigeono.io)
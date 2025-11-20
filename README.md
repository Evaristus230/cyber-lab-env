# 🔐 Self-Contained Pentest Lab

> A Docker-based environment for practicing web app penetration testing — no VMs, no setup headaches.

This lab includes:
- 🍹 **OWASP Juice Shop** — modern vulnerable web app  
- 🛡️ **OWASP ZAP** — headless scanning & API access  
- 🖥️ **Portainer** *(optional)* — container management GUI  

Built for **repeatability**, **learning**, and **toolchain integration**.

---

## 🚀 Quick Start

1. **Clone this repo**:
   ```bash
   git clone https://github.com/Evaristus230/cyber-lab-env.git
   cd cyber-lab-env

   docker-compose up -d

   Access services:
🍹 Juice Shop: http://localhost:3000
🛡️ ZAP API: curl http://localhost:8090/JSON/core/view/version/
🖥️ Portainer: http://localhost:9000 (set admin password on first launch)

docker-compose down

💡 Why I Built This
During my cybersecurity training, I struggled with inconsistent lab setups — broken VMs, port conflicts, missing tools.

This lab solves that by:

✅ Isolating services in containers
✅ Pre-configuring ZAP for automation (e.g., CI/CD integration)
✅ Allowing quick reset with docker-compose down && up
✅ I use this daily for: 

Testing gobuster + sqlmap workflows
Simulating full recon → exploit → report cycles
Training on modern app vulnerabilities (JWT, SSRF, XXE)

# Overwrite the README with the correct AEGIS Python scanner version
cat > README.md << 'EOF'
# 🛡️ AEGIS - Autonomous Security Scanner

**Python-based security scanner for open ports and vulnerabilities**

[![License: AGPLv3](https://img.shields.io/badge/License-AGPLv3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![GitHub stars](https://img.shields.io/github/stars/Leodrik-security-org/L-Core)](https://github.com/Leodrik-security-org/L-Core/stargazers)

---

## 🚀 Quick Start (30 seconds)

```bash
# Clone the repository
git clone https://github.com/Leodrik-security-org/L-Core.git
cd L-Core

# Run your first security scan
python3 -m src.aegis.core.engine

# See demo mode (simulates findings)
python3 -m src.aegis.core.engine --test
🔍 What AEGIS Scans
Port	Service	Severity	Risk
21	FTP	MEDIUM	Anonymous login, clear text
22	SSH	MEDIUM	Weak credentials, brute force
23	Telnet	🔴 CRITICAL	Completely insecure, use SSH
25	SMTP	MEDIUM	Open relay, spam relay
80	HTTP	LOW	Missing HTTPS, mixed content
443	HTTPS	LOW	SSL/TLS misconfigurations
8080	HTTP-Alt	LOW	Development servers exposed
3389	RDP	🟠 HIGH	Remote Desktop exposed
5900	VNC	🟠 HIGH	No authentication, clear text
27017	MongoDB	🟠 HIGH	No authentication by default
📊 Example Output
text
============================================================
  🛡️  AEGIS Security Scanner v0.1.0
  Autonomous Enterprise Guardian & Intelligence System
============================================================

🔍 Scanning target: 127.0.0.1
🎮 TEST MODE - Simulating findings for demonstration

⚠️  Found 3 open ports:
   • Port 80: HTTP - LOW
   • Port 443: HTTPS - LOW  
   • Port 8080: HTTP-Alt - LOW

💾 Saving results to database...
📊 Generating report...

✅ Scan complete!
   📄 Report: aegis_report.json
   💾 Database: aegis.db

🔧 Recommendations:
   ℹ️  Web server exposed. Ensure HTTPS and proper security headers.

============================================================

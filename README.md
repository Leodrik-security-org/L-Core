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

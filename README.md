# elastic-home-soc
# Home SOC in a Box with Elastic Stack

A complete home Security Operations Center (SOC) running on a Raspberry Pi, providing enterprise-grade endpoint detection and response (EDR) capabilities for your home network.

## What This Does

- **🛡️ Endpoint Protection**: Real-time monitoring of file changes, process execution, and network activity
- **🔍 Security Analytics**: Centralized logging and analysis of security events
- **📊 Visualization**: Professional security dashboards and investigation tools
- **🚀 Fleet Management**: Centralized agent deployment and policy management
- **💰 Enterprise for Free**: Full Elastic Stack capabilities at zero cost

## Quick Start

**Hardware Requirements:**
- Raspberry Pi 4/5 with 8GB RAM (minimum)
- 128GB+ microSD card
- Ethernet connection (recommended)

**Setup:**
```bash
git clone https://github.com/one3qualsone/elastic-home-soc.git
cd elastic-pi-soc
nano .env  # Configure passwords and settings
docker compose up -d es01 kibana setup
# Wait 5 minutes for services to start
docker compose up -d fleet-server
```

**Access:**
- Kibana: `https://your-pi-ip:5601`
- Username: `elastic`
- Password: From your `.env` file

## What You Get

- **Elasticsearch**: Data storage and search engine
- **Kibana**: Web interface for security analysis
- **Fleet Server**: Agent management and policy deployment
- **Elastic Defend**: Enterprise EDR capabilities
- **Complete tutorial**: Step-by-step setup and troubleshooting guide

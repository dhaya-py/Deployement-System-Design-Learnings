# 📘 DEPLOYMENT NOTES — LOGGING & PROCESS MANAGERS
## 🔹 1. Logging

Servers must keep logs to track:

Errors
Warnings
Info
Requests

Example Python logging:

import logging
logging.basicConfig(level=logging.INFO)
logging.info("App started")

## 🔹 2. Process Managers

Used to keep FastAPI alive:

systemd

supervisor

pm2 (for Node but concept is same)

Example systemd service:

[Service]
ExecStart=uvicorn main:app --host 0.0.0.0 --port 8000
Restart=always

## 🔹 3. Log Locations (Linux)

Logs are stored in:

/var/log/
/var/log/nginx/
/var/log/syslog

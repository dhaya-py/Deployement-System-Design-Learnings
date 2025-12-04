# Day 2 Backend Notes

## 1. Processes

A process = running program instance
Example: python main.py runs as a process.

## 2. Ports

Every backend listens on a port:

80 = HTTP

443 = HTTPS

8000 = FastAPI default

5000 = Flask

Example:

http://127.0.0.1:8000/

## 3. Services

In production, services keep your backend alive:

systemd

PM2

Supervisor

## 4. Server Flow

When someone visits your site:

User → DNS → Load Balancer → Server → Port → Backend → Response
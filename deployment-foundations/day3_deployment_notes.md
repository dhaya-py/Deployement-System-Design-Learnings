# 📘 DEPLOYMENT LEARNING NOTES
## 🔹 1. Environments

Environment   	Purpose
Dev     	  Local development
Stage	      Testing / QA environment
Prod	      Live server

## 🔹 2. Environment Variables (.env)

Used to store secrets like:

DB_PASSWORD=...
SECRET_KEY=...
API_KEY=...


Never hardcode secrets.

## 🔹 3. Secrets Management

Options:

.env file

Docker Secrets

AWS Secrets Manager

Environment variables in server

## 🔹 4. Why environments matter

You DO NOT want:

Debug mode in production

Local database in production

Local API keys on server
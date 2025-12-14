# 📝 DEPLOYMENT TASKS
## ✔ Easy

### What is logging?

logging is the only way to know what our backend is doing when we are not watching. 

types of logs - ERROR, WARNING, INFO, REQUEST

### Why do we use logging?

Tracks everything.
without log :

we can't debug, we can't audit, we can't analyze performance, we can't detect attacks

## ✔ Medium

### Write the 4 logging levels

error   - something broke. ex: ERROR : database connection lost

warning - something might become a problem. ex: WARNING : low memory, slow query detected

info - normal behaviour, getting information. ex: INFO : spp started, user signed up

request - every request hitting our API.  REQUEST : GET user/data 200 ok

## ✔ Hard

### Describe how you will log your FastAPI backend in production:


In production, I will set up a structured logging system for FastAPI with separate log files:

1. API Logs (INFO level):
   - Track normal operations such as app start, route loading, database connections.
   - Logged into logs/api.log.

2. Error Logs (ERROR level):
   - Capture exceptions, database errors, and crashes.
   - Logged into logs/error.log as a dedicated error logger.

3. Request Logs (via middleware):
   - Every incoming request is logged with method, endpoint, status code, and response time.
   - Logged into logs/requests.log.

4. Separate Log Files:
   - api.log → general info
   - error.log → errors only
   - requests.log → request audit trail
   This keeps logs clean and easy to debug.

5. Log Rotation:
   - Use logrotate to rotate logs daily, compress old logs, and prevent disk growth.

6. Process Manager:
   - systemd or supervisor captures startup/shutdown logs via journalctl.

This logging structure ensures clean debugging, monitoring, and production stability.

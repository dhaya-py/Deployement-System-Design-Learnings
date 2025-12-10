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

API logs

error logs

request logs

separate log files
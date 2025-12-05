# 📝 DEPLOYMENT TASKS
## ✔ Easy

 ### Define “port”

 A port = a "door number" through which app communicates over the network

 IP = buiilding
 Port = door number
 Protocol = rules for how to talk through door number.
 
 Every backend listens on a port ;

 80 - HTTP
 443 - HTTPS
 8000 - FastAPI 
 5000 - Flask


 ### Define “process”

 Process = running program instance. example : python main.py run as process.

 process = running instance of a program

 if you run - python main.py

 your OS creates : program instruction in memory, PID (process ID), CPU + RAM allocates for it.

 for example : you run - uvicorn main:app --reload, your OS run one process - uvicorn (2417), if you scale for 3 workers, then your OS run
               uvicorn worker1
               uvicorn worker2
               uvicorn worker3

## ✔ Medium

 ### Write: “How FastAPI runs on port 8000 on a server”

 In a server, I upload my fastapi app then I create a service for running my program in the server automatically and auto restart instead of
 manually running everytime, If I run manually - if terminal close : app stops, if server update or crash : app doesn't auto restart.
 FastAPI default port is 8000 so it communicates over the network.

## ✔ Hard

 ### Write how you will run your first backend:

Start process  - In backend, I will create a program and named it as main.py, now my server process is running that program, my OS creates
                 program instructions in memory, PID (process id), CPU + RAM allocates for program. it run a program as uvicorn (2174)

Use a service  - In production, services used for automatically and actively run our program instead of manuall run everytime

Serve via domain  -  User access our URL and send request, DNS checks domain -> IP.

Client sends request.
DNS check domain -> IP.
Server receives request.
runs business logic.
Queries DB.
Retrieves data.
Formatting response.
Return JSON response.
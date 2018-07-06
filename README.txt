
To make it distributed system, communication between different node process are being done by socket.

Steps to run this program:

>git clone https://github.com/veeragiri/task.git
>cd task
>npm install

Open n terminal, let's say n = 4 for now.

Terminal 1> node DBServer.js

Terminal 2> node app.js 8081

Terminal 3> node app.js 8082

Terminal 4> node app.js 8083



Terminal 2> curl localhost:8081/set/key1344 -d "value=value"

Terminal 3> curl localhost:8082/get/key1344
value

Terminal 3> curl localhost:8083/get/key1344
value



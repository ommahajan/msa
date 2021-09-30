# msa
8) jenkins
-----------

docker pull jenkins/jenkins:lts
docker volume create jenkins
docker run --restart=always -d -p 8051:8080 -p 50000:50000  --net=local-network -v /home/jenkins:/jenkins --name=jenkins jenkins/jenkins:lts
Now admin user is created with password in console.
http://localhost:8051/
Now unlock the jenkins by password given in console.



http://localhost:8041/authenticate
http://localhost:8041/producer/employee
http://localhost:8041/consumer/employee
http://localhost:8041/consumer/health-check
http://localhost:8041/producer/getEmployeeList
http://localhost:8090/zuul-service/dev/v1.0

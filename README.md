# tomcatwar-demo2

This repo will create a .war file to deploy into tomcat server

before we begin :
-----------------
jenkins server (either in local machine/docker container)
Tomcat server (docker)
Jenkins plugin needed : Deploy to container
Build tool: Maven 
Jdk 8

Git repo : https://github.com/rjshk013/tomcatwar-demo2

Maven Goals: clean install

Tomcat configuration:
WAR/EAR files: **/*.war
Context path: rps
Containers: Tomcat 8.x
Tomcat URL: http://ip:portno
(If your tomcat is in local machine ,give localhost ,if it is docker give local machine ip)

Configure credentails for tomcat server : I have given username & password as deployer

After the build check the war file generated from the jenkins folder (/var/jenkins_home/jobs/job-name/workspace/target/

At last check the war file deployed correctly from the tomcat url like : localhost:port/rps 

Reference : https://www.theserverside.com/video/Step-by-step-Jenkins-Tomcat-deploy-of-a-WAR-file

Tomcat-wardemo 3
-----------------

You can clone the repo : https://github.com/manishmore/JenkinsWar

To get the app on tomcat : http://localhost:8999/JenkinsWar/

follow blog : https://cmstoddler.com/deploy-war-file-tomcat-8-using-jenkins-maven-and-github

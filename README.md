# Jenkins-CICD


In this project we are going to install Jenkins on a ec2 server and integrate Github with jenkins thru a web hook and do continuous integration and continuous delivery/deployment.

Before installaling Jenkins on a server first we need to install Java .

steps to install Jenkins on a server

Create AWS EC2 instance
      sudo apt update
      sudo apt install openjdk-11-jre
      java -version
      curl -fsSL https://pkg.jenkins.io/debian/jenkins.io.key | sudo tee \   /usr/share/keyrings/jenkins-keyring.asc > /dev/null 
      echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \   https://pkg.jenkins.io/debian binary/ | sudo tee \   /etc/apt/sources.list.d/jenkins.list >             /dev/null
      sudo apt-get update 
      sudo apt-get install jenkins
      systemctl status jenkins
   
   
   ![image](https://user-images.githubusercontent.com/92623347/232256098-5294af33-fb99-418e-a1b3-04fc97b2e3bb.png)

Now if you want to accessJenkins we need to open port 8080 by adding inbound rule in our Ec2 security group.

Then we can access Jenkins only admin password(for the first time) which we get here

cat /var/lib/jenkins/secrets/initialAdminPassword


![image](https://user-images.githubusercontent.com/92623347/232256311-63735d7b-8aa0-4db0-bf87-282705c55dc3.png)

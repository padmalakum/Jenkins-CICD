In this we will connect Jenkins-master to agent to run the jobs

For this we need to go into ./ssh folder and copy public  id_rsa key of master server and paste it in authorized keys file of agent server

then Master and agent are connected thru ssh.

![image](https://user-images.githubusercontent.com/92623347/232556097-11f01fb8-7aa5-43dc-acb0-d90c58b1256f.png)

![image](https://user-images.githubusercontent.com/92623347/232556318-c533d86a-af94-4d7f-913c-af2bce99c25e.png)

![image](https://user-images.githubusercontent.com/92623347/232556697-8d00dcc5-887b-423f-8117-6347fde7488a.png)

Next we need to connect agent in jenkins

you need to add the node in the form to create  a new agent

give all the details for the node  to connect to master and install java on the agent so that it will connect

![image](https://user-images.githubusercontent.com/92623347/232559980-383cf184-eb74-4382-8344-2ef00ba13425.png)


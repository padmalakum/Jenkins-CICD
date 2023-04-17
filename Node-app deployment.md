Here we will see how to deploy Node app deployment automatically.

First we need to integrate Github with jenkins by creating a webhook in github repository

In the repository setting we need to give our jenkins url to create a webhook

![image](https://user-images.githubusercontent.com/92623347/232325237-c3aacae2-6f2f-4443-9d4c-83afc13efb27.png)

and then we  select these settings in Jenkins configure

we need to select github hook trigger for GITscm polling  so that it will connect to github

and execute shell commands .

![image](https://user-images.githubusercontent.com/92623347/232325478-5d148a00-034e-48af-a0a2-98d9007a3207.png)

and when you change anything in your code in github and commits ,webhook automatically triggers and runs the build resulting new changes inthe deployment
![image](https://user-images.githubusercontent.com/92623347/232554227-3dc0f2c5-4b78-490c-ac1d-23e1b3d1e7b9.png)





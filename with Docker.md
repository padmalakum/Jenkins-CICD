now we need to add docker build steps .
![image](https://user-images.githubusercontent.com/92623347/232259563-46beb3d6-b1e0-4471-af7a-c96fc9dc3ec3.png)

and install jenkins on our Ec2 server and give permissions as sudo usermod-aG docker jenkins

and click build now

![image](https://user-images.githubusercontent.com/92623347/232259618-1df0d757-12a3-42fc-a385-79350269987f.png)

![image](https://user-images.githubusercontent.com/92623347/232259631-adb07775-0438-4052-95c2-be130b5e3930.png)

we can see our images and container here also


![image](https://user-images.githubusercontent.com/92623347/232259683-ffcb6877-c5c4-42e7-9f07-f67b1478a709.png)

and we need toopen 8001 port as we exposed that port in our dockerfile for that app

and our app looks like this

![image](https://user-images.githubusercontent.com/92623347/232259727-3f13e1ff-b4c8-4c83-85d6-6e5c8ee6369a.png)

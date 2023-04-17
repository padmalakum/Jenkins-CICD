In this we will create Environmental variables by installing plugin in jenkins and define our docker username and password and use these in our pipeline script to push images to docker hub.

First we need to add docker credentials in manage jenkins by creating a id for it 

![image](https://user-images.githubusercontent.com/92623347/232615415-cb537771-5d32-400e-81fb-045408247473.png)
 and then we can use these by creating environmental variables for username and password 
 ![image](https://user-images.githubusercontent.com/92623347/232615903-a4925c1d-3b30-4f3f-a467-254293d7c910.png)

andwe can write the script by using withCredentials in groovy
![image](https://user-images.githubusercontent.com/92623347/232616167-2f3f3388-5dfb-4eed-8ca6-45ba3aa29605.png)

and attaching webhook for this creates an automated CI/CD pipeline by pushing image to docker and pulling that image from dockerhub to deploy on our ec2-instance

![image](https://user-images.githubusercontent.com/92623347/232616470-70df01e7-1302-47c9-bc00-8a448e43eada.png)

and we can run the app in on our agent dev

![image](https://user-images.githubusercontent.com/92623347/232616677-779a547f-cc2f-49d7-af2f-4141aa525e4c.png)


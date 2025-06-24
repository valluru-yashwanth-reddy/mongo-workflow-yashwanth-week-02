# yashwanth-github-workflow
---> Firt  we create a pipeline for the automate of the running and installation of docker inside our EC2 instance ,and for the building image and running to the container.
---> For this we need to create a docker hub image ,and then we generate a new access token from the github .
--> then we create a github repository with the ci/cd pipeline  then along with this we upload our files app.js  and package.json.
--> along with this we create a new ec2 instance called yashwanth-github-actions.
--> we add Our credentials (ec2-host,ssh key,token generated from the github(this can be viewd only once after generated))these mentioned credentials are added in the secrets.
--> then we ssh into the instance "yashwanth-github-actions "and we install docker in it and give privilege to the current user to run docker commands logout and login to apply this chanages made.
![Screenshot 2025-06-21 225533](https://github.com/user-attachments/assets/48e9e495-1d41-493d-a11b-b05dc45ea78b)
![image](https://github.com/user-attachments/assets/69538f34-7925-43c5-a508-6f62f0b626a4)
![image](https://github.com/user-attachments/assets/bfd617f1-ee55-41b0-8573-cae1669e9820)
![image](https://github.com/user-attachments/assets/7656bc8b-fd58-4fed-9f96-9918bb3e6edb)
 ![image](https://github.com/user-attachments/assets/0c6b6f56-3873-408c-a10d-580aa2fde125)





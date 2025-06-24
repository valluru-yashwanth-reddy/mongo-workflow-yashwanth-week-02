First, we set up a secure place called secret to store the admin user and secret key, which we get with a command.
--> Then we create a secret.yaml file with apiVersion v1 and kind Secret including the admin user and key details and run kubectl apply -f secret.yaml to create it.
--> Next we launch MongoDB using a Deployment with apiVersion apps/v1 and a Service with apiVersion v1 to give it a fixed address applying them with kubectl apply -f.
--> We also make a ConfigMap for non-sensitive data like settings and apply it.
--> For the backend we deploy Mongo Express with an external Service, adding basic authentication for the admin user and password by linking to our secret.
--> To see everything we run kubectl get all to list all resources. To access Mongo Express we use minikube service mongo-express or kubectl get svc mongo-express to get the URL which might open the browser. 
--> After logging in with the admin credentials we can manage databases in Mongo Express. 
--> When finished we clean up by deleting resources with kubectl delete -f or specific delete commands

![Screenshot (28)](https://github.com/user-attachments/assets/68934774-52c3-4a71-a412-f0658cd26f5e)
![Screenshot (27)](https://github.com/user-attachments/assets/bd10ed57-1f75-4e20-a3fe-e74264ac3f2a)
![Screenshot (26)](https://github.com/user-attachments/assets/4bbf49e3-7213-4941-a0e5-d24f7ec7d3b2)
![Screenshot (25)](https://github.com/user-attachments/assets/cc6756df-50ad-4e5b-ae62-7d69b4fddf40)





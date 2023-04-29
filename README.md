to run the application-
1. create docker image of an application and push to docker hub 
2. create Kubernetes deployment configuration file and service configuration file for the application
3. run the following  commands-
 a. kubectl apply -f dashboard-adminuser.yaml ( to create admin user)
 
 b. kubectl apply -f cluster_role_binding.yaml 
 c. kubectl apply -f createDeployment.yaml
 d. kubectl apply -f firstservice-service.yaml
 e. kubectl apply -f createPod.yaml
 f. kubectl -n kubernetes-dashboard create token admin-user ( to get token )
 g. kubectl proxy ( to start the kubernetes dashboard)
4. go to kubernetes dashboard and paste the token 
5. now we can see our deployed application in the kubernetes dashboard

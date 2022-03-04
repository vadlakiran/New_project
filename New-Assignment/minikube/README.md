#TO run the react js app run the below commnad
kubectl create -f sys-stats-react-deploy.yml
#kubectl create -f python_deployment.yml
#After that expose node port using below command
#kubectl expose deployment react-deployment --type=NodePort --port=3000 --name sys-stats-react-service -o yaml > sys-stats-react-service.yml
#kubectl expose deployment python-deployment --type=NodePort --port=5000 --name python-service -o yaml > python_service.yml
#To Run Ingress 
#kubectl create -f ingress.yml
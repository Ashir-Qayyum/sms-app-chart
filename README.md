Student Management System

Cloned from: https://github.com/medinar/full-stack-spring-boot-react.git

To practice creating custom helm repo to deploy SMS App on k8s cluster using helm for hands on poc

First add the repo, run:

helm repo add sms-app https://Ashir-Qayyum.github.io/sms-app-chart

helm repo update

Then deploy one-by-one:

helm install sms-postgres sms-app/sms-postgres

helm install sms-backend sms-app/sms-backend

helm install sms-frontend sms-app/sms-frontend

The frontend is configured to run at port 80, however, port-forwarding can
be done to access at any different port in local
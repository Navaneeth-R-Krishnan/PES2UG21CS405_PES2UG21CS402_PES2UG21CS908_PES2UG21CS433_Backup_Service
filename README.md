# back-up-service - Backing up files in an interval basis, using CRON


WEEK-1:

>Created a GCP account and set up google-drive api
>
>Created a python script to backup files from "backupfiles" directory
>
>Created a docker container to run this script with necessary dependencies installed
>
>cmd: docker build -t back-up-service

WEEK-2:

>set up cronjob in kubernetes
>
>set up logging

##command sequence
1. minikube start
2. kubectl apply -f backup_pvc.yaml
3. kubectl apply -f backup_cronjob.yaml
check if running:
kubectl get jobs
kubectl delete cronjob backup-cronjob


# App 2 Image Build and Deploy in Cluster with YAML

** Image Build and Push to Repo
>docker build -t mizapp2 .
>docker tag mizapp2:latest dockerhubrepo:tag
>docker push dockerhubrepo:tag

Make sure Dockerfile and app src file is in same folder.

**Node Selection
To select the node selector we need to label the nodes

>kubectl label nodes hostname app2-deploy=true --overwrite

**Image Deploy
you can set the folder location ot you can go to the folder and deploy Like that.

>kubectl apply -f BrainStationTest/Task1/app2/deploy/app2deploy.yaml
>kubectl apply -f BrainStationTest/Task1/app2/deploy/app2service.yaml

As there is no DB/redis server,,just a normal app so there is no config.yaml
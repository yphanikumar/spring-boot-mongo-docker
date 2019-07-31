# Jenkins commmands

    export AWS_ACCESS_KEY_ID=AKIAUJCFGHJKDOC2VY6Y

    export AWS_SECRET_ACCESS_KEY=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

    export AWS_DEFAULT_REGION=us-east-1

    aws eks --region us-east-1 update-kubeconfig --name test-cluster

    kubectl get nodes

    kubectl apply -f spring-deploy.yaml

    #kubectl set image deployment spring-deployment springboot=phanikumary1995/test-app-${BUILD_NUMBER} --record

    kubectl get pods

    kubectl get svc

    kubectl get deployments

    kubectl rollout status deployment spring-deployment


# Build Project Using Maven

Maven is java based build tool to generate executable 

packages(jar, ear,war) for java based projects.

```bash
mvn clean package
```

## Create Docker Image
Docker is a continerization tool.Using docker we can deploy our applications as 

containers using docker images. Containers contains application code and also the softwares,

config files whatever is required for our application to run.

Create docker image using Dockerfile


```docker
docker build -t dockerhandson/spring-boot-mongo .
```

## Deploy Application Using Docker Compose 

```docker-compose 
docker-compose up -d 
```

## List Docker Containers
```docker
docker ps -a
```

## License
[Mithun Technologies](http://mithuntechnologies.co.in)

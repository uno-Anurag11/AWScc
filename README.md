# AWScc
## What is cloud computing
- cloud computing is the delivery of computing services including servers,storage,databases,networking,software etc.
## benfits 
- faster time to market
- scalability and flexibility
- cost savings
- better collaboration
- advanced security
- data loss prevention
## disadvantage 
- risk of vendor lock-in
- less control over underlying cloud insfra
- concerns about security risks like data privacy and online threats
- integration complexity with exisiting systems
- unforseen costs and unexpected expenses

![Screenshot from 2023-11-26 11-13-28](https://github.com/KRIISHSHARMA/AWS/assets/86760658/5cb528d2-0305-4def-af70-743624f9f1e5)

![Screenshot from 2023-11-26 11-14-43](https://github.com/KRIISHSHARMA/AWS/assets/86760658/72395079-6a3a-4a2d-a61a-e9a23fb50506)

- example of private implementation softwares : openstack , opennebula 


## Hyperscalars : A hyperscaler is a type of large-scale data center that offers massive computing resources, typically in the form of an elastic cloud platform. Organizations use them to deploy and manage large-scale applications and services.

![Screenshot from 2023-11-26 11-17-36](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a37cc108-bf86-481f-80cd-ea7ec4b1e5a1)

![Screenshot from 2023-11-26 11-19-52](https://github.com/KRIISHSHARMA/AWS/assets/86760658/7f6c1e83-29b4-43dc-9cf5-2e20cdc321fa)

## Compute services 
- EC2  
- ECS/EKS : containerized services `
  - Fargate
- lambda : serverless 

## Storage Services
- S3
- EBS : Amazon Elastic Block Storage is a storage service wherein each block of storage acts like a separate hard drive (volume) . 
- EFS : dont need to assign any volume , can do on its own , seamless storage , database on EC2 instances 
- Archival service - Glacier : Amazon Glacier is extremely low cost, secure, and durable storage service for data archiving and
backup. That data stored which are not needed instantly , eg old data . Takes time min 4 hours or 1 day to retrieve request ( S3 instantly returns request)

## Network Services
- VPC : own insolated environment in a public cloud
- Domain Name Service - Route 53

![Screenshot from 2023-11-26 17-59-50](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a6881e65-16b5-4e2f-8480-973fee9344f6)

- public subnet : can receive traffic from outerworld 
- private subnet : cannot receive traffic from outerworld but may or may not send traffic to outerworld

![Screenshot from 2023-11-26 18-03-33](https://github.com/KRIISHSHARMA/AWS/assets/86760658/dee853ad-6c86-4238-98ec-ba7ba60b7831)
![Screenshot from 2023-11-26 18-05-39](https://github.com/KRIISHSHARMA/AWS/assets/86760658/0e807497-f6ce-484e-82c0-40f1bcd83c45)


![Screenshot from 2023-11-26 13-40-57](https://github.com/KRIISHSHARMA/AWS/assets/86760658/3dcafdd0-84f9-4ecd-9843-e6ea71061a3f)
![Screenshot from 2023-11-26 13-46-08](https://github.com/KRIISHSHARMA/AWS/assets/86760658/2ba98aae-9871-40a1-89a9-3bbcaa961fdc)
![Screenshot from 2023-11-26 13-47-33](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a7b8c06a-c163-4b80-a052-d433928260ff)
![Screenshot from 2023-11-26 13-57-52](https://github.com/KRIISHSHARMA/AWS/assets/86760658/86722cee-9cc8-47be-9e62-a4f6fb8dc842)
![Screenshot from 2023-11-26 13-59-20](https://github.com/KRIISHSHARMA/AWS/assets/86760658/2edee858-bceb-49da-8c19-d87403bf0582)

- **Apache web server works on layer 7 , using single apache server one can deploy multiple applications on different ports based on paths (URLbased) (virtual hosts) . virtual hosting can only work on layer 7**

## Application based LB 
- key pair : kind of like a password (public key is username; private key is password)
  - PPK (PuTTY Private Key) and PEM (Privacy Enhanced Mail) are two file formats that are commonly used for SSH and SSL/TLS connections. While PPK files are primarily used with PuTTY on Windows, PEM files are more widely supported and can be used with various tools and platforms

- security groups : A security group controls the traffic that is allowed to reach and leave the resources that it is associated with. For example, after you associate a security group with an EC2 instance, it controls the inbound and outbound traffic for the instance. When you create a VPC, it comes with a default security group. (acts as a firewall)

![Screenshot from 2023-11-26 15-39-41](https://github.com/KRIISHSHARMA/AWS/assets/86760658/90eeb7f4-8428-4876-8a3e-288feb952aa1)
![Screenshot from 2023-11-26 15-39-41](https://github.com/KRIISHSHARMA/AWS/assets/86760658/73bc04f3-081a-4451-adf4-f89c488b8a67)
![Screenshot from 2023-11-26 15-40-34](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e96e05df-b33c-400a-8264-946d9a878644)
![Screenshot from 2023-11-26 15-40-51](https://github.com/KRIISHSHARMA/AWS/assets/86760658/bb9edf0e-42cb-49b8-abe9-34f0c2d35e87)

### Creating a target group 
- Your load balancer routes requests to the targets in a target group and performs health checks on the targets.
- LB routes traffic to target group then traffic group routes traffic to the back end ec2 instances or IP addresses etc

![Screenshot from 2023-11-26 15-49-16](https://github.com/KRIISHSHARMA/AWS/assets/86760658/eff46d2f-b504-44e9-9269-7a2b877930d6)
![Screenshot from 2023-11-26 15-49-16](https://github.com/KRIISHSHARMA/AWS/assets/86760658/5500b66f-9467-4353-9599-5186bcbb156a)
![Screenshot from 2023-11-26 15-50-48](https://github.com/KRIISHSHARMA/AWS/assets/86760658/848472d8-4fda-4580-9563-d10d1e17202c)

![Screenshot from 2023-11-26 16-19-25](https://github.com/KRIISHSHARMA/AWS/assets/86760658/bb5bbe47-681f-4383-8825-a3974aef26a4)
![Screenshot from 2023-11-26 16-24-54](https://github.com/KRIISHSHARMA/AWS/assets/86760658/f9a7faaf-0855-4cc3-afa5-fc65e9793b22)

## Autoscalling 
![Screenshot from 2023-11-26 16-44-57](https://github.com/KRIISHSHARMA/AWS/assets/86760658/7dc2321e-8595-4bd4-8c6e-b3696e5a6999)

### Creating launch template
![Screenshot from 2023-11-26 16-59-20](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1ee051f9-5524-4a61-985b-4cbe32bee5ee)
![Screenshot from 2023-11-26 17-01-18](https://github.com/KRIISHSHARMA/AWS/assets/86760658/ce935d36-35b6-4fbf-8662-d4e0ccb17fcc)
![Screenshot from 2023-11-26 17-17-33](https://github.com/KRIISHSHARMA/AWS/assets/86760658/8aee6470-e044-437e-a5f8-8811d748f1f0)
![Screenshot from 2023-11-26 17-19-34](https://github.com/KRIISHSHARMA/AWS/assets/86760658/884c3f5a-4104-46f1-b197-164ce1cf29e4)


![Screenshot from 2023-11-26 17-05-17](https://github.com/KRIISHSHARMA/AWS/assets/86760658/b3b85552-b55e-4e5d-bb8e-b221add8bc17)
![Screenshot from 2023-11-26 17-08-50](https://github.com/KRIISHSHARMA/AWS/assets/86760658/b7f17b5a-3a38-4cf3-a754-fca7fc871c01)
![Screenshot from 2023-11-26 17-11-22](https://github.com/KRIISHSHARMA/AWS/assets/86760658/8fe1d28f-e615-48f4-8e19-c1e6932263e2)
![Uploading Screenshot from 2023-11-26 17-22-51.png…]()


### Creating scalling policies 
![Screenshot from 2023-11-26 17-34-29](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1e2b5ae4-2379-4a52-a3d8-687e9e1bf3cd)
![Screenshot from 2023-11-26 17-35-23](https://github.com/KRIISHSHARMA/AWS/assets/86760658/8cead298-7c0e-4f1d-878e-ef6792825f03)

## Artificial load 
``` bash
htop
```
![Screenshot from 2023-11-26 17-39-48](https://github.com/KRIISHSHARMA/AWS/assets/86760658/c6aa182a-0282-45f5-b610-c3aad12e57cd)

- currently 0

- making instance count to a high number
``` bash
seq 999999999999999999999 > /dev/null &
```
![Screenshot from 2023-11-26 17-43-25](https://github.com/KRIISHSHARMA/AWS/assets/86760658/93d6f92d-ba24-4e4a-8f2e-5901802d18f0)

![Screenshot from 2023-11-26 17-58-10](https://github.com/KRIISHSHARMA/AWS/assets/86760658/88495da3-fbbe-4e66-bfc3-94c81d92787c)
![Screenshot from 2023-11-26 17-58-29](https://github.com/KRIISHSHARMA/AWS/assets/86760658/00cd991a-994e-4890-9176-adb65dbf3ccd)
![Screenshot from 2023-11-26 18-11-32](https://github.com/KRIISHSHARMA/AWS/assets/86760658/7ce90daa-db12-4b4c-b655-ba62d155f060)

- going to the DNS name and reloading will take you to diff targets(3)
- this is **round robin** at work  

## AWS CLI : The AWS Command Line Interface (AWS CLI) is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.
- BOTO library in python

![Screenshot from 2023-11-27 16-45-38](https://github.com/KRIISHSHARMA/AWS/assets/86760658/fae33c2d-6122-4ee2-aa75-5f061bcbba20)
![Screenshot from 2023-11-27 16-47-42](https://github.com/KRIISHSHARMA/AWS/assets/86760658/768d5a91-8c74-42ed-b08e-14c3ad5c11eb)

``` bash
sudo snap install aws-cli
```
``` bash
aws configure
```
![Screenshot from 2023-11-27 17-08-27](https://github.com/KRIISHSHARMA/AWS/assets/86760658/71a8036d-299a-4b48-adbb-8049b3f16dea)

- in security credentials , before creating access key copy and paste PU , PrK and fill location and format in terminal 
- give user access

![Screenshot from 2023-11-27 17-30-18](https://github.com/KRIISHSHARMA/AWS/assets/86760658/50c16ed9-0a30-49a2-b9aa-d834c2622e99)

![Screenshot from 2023-11-27 17-31-17](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a7ce2566-0cbb-4b6e-8412-106c939a0f81)
![Screenshot from 2023-11-27 17-31-32](https://github.com/KRIISHSHARMA/AWS/assets/86760658/cb651886-272d-4b28-94de-25785de9fcab)

- after creating instance
``` bash
aws ec2 describe-instances
``` 

![Screenshot from 2023-11-27 17-35-01](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e4ba62f0-42f5-4e8d-840f-41d32e1cf6a3)
![Screenshot from 2023-11-27 17-35-01](https://github.com/KRIISHSHARMA/AWS/assets/86760658/de7fef08-39e8-4525-a276-6da3f8c2e742)
![Screenshot from 2023-11-27 17-46-10](https://github.com/KRIISHSHARMA/AWS/assets/86760658/15f77e24-064b-4aca-9de0-562c6a54c890)
![Screenshot from 2023-11-27 18-12-04](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1cf4f02a-59c8-43d9-896f-28d980add612)
![Screenshot from 2023-11-27 18-12-32](https://github.com/KRIISHSHARMA/AWS/assets/86760658/6e9a8d71-0ede-42fd-9c93-3a53a2e109a0)
![Screenshot from 2023-11-27 18-14-02](https://github.com/KRIISHSHARMA/AWS/assets/86760658/899d441d-7208-4778-8537-6be1a92008d0)
![Screenshot from 2023-11-27 18-17-35](https://github.com/KRIISHSHARMA/AWS/assets/86760658/89a6f2f4-a014-4ec6-91fe-4994d0e26d40)
![Screenshot from 2023-11-27 18-26-06](https://github.com/KRIISHSHARMA/AWS/assets/86760658/4789776e-d9e7-4a27-8c3d-038298c02daf)


- docker image to create art load
- pods : Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers.

 ![download](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1bf8d1eb-e0b6-4674-bd98-fbcf383135d3)

- daemon sets : works on nodes where pods are running , can manage all your agents eg if we are runninf 5 ec2 instances behind the k8s cluster then we can run 1 daemon set and that daemon set wil take care of all the agents 

## CLOUD 9
- cloud based IDE (vscode , pycharm etc)
- provides IDE on browsers

![Screenshot from 2023-12-02 16-01-33](https://github.com/KRIISHSHARMA/AWS/assets/86760658/9208cded-f435-451a-a192-c4a254244e75)
![Screenshot from 2023-12-02 16-12-26](https://github.com/KRIISHSHARMA/AWS/assets/86760658/9efd1bc2-5393-4ac1-9a28-0355a7961482)
![Screenshot from 2023-12-02 16-12-51](https://github.com/KRIISHSHARMA/AWS/assets/86760658/b7a5eecb-5d92-46af-a9ad-7ba6db2a5391)


- after confiugring aws cli on cloud 9 (scroll up) 
-  configure EKS ctl and kubectl [link for installation](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/setting-up-eksctl.html)
  
![Screenshot from 2023-12-02 16-35-44](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e128f431-c888-4cc3-b8fa-2f7a0a3835a1)
![Screenshot from 2023-12-02 16-55-57](https://github.com/KRIISHSHARMA/AWS/assets/86760658/79d1bb3c-b8b3-49af-bd3f-b7552ab700da)
![Screenshot from 2023-12-02 16-56-13](https://github.com/KRIISHSHARMA/AWS/assets/86760658/9e89cf9d-7dbc-419e-8f0b-f35c8b830198)
![Screenshot from 2023-12-02 16-57-22](https://github.com/KRIISHSHARMA/AWS/assets/86760658/7bd6650b-e499-414d-baef-5f7a5bdc8799)

- launching a cluster
  ```bash
  eksctl create cluster --name test --version 1.28 --nodegroup-name ng.default --node-type t3.micro --nodes 2 --managed
  ```
  ![Screenshot from 2023-12-02 17-05-19](https://github.com/KRIISHSHARMA/AWS/assets/86760658/460b3b95-798a-439f-9611-95c419fa1064)

- yaml file for nginx container launched with official nginx image
  ``` bash
     apiVersion: apps/v1
  kind: Deployment
  metadata:
      labels:
          environment: test
      name: test
  spec:
      replicas: 1
      selector:
          matchLabels:
               environment: test
      template:
          metadata:
              labels:
                  environment: test
          spec:
              containers:
              - image: nginx:1.16
                name: nginx

  ```
``` bash
  nano nginx-deployment.yaml
```
- kubectl is the thing using which we will be creating , launching the resources , creating pods , troubleshooting cluster using kubectl
- we will apply this file using kubectl
  ``` bash
    kubectl apply -f nginx-deployment.yaml
  ```
![Screenshot from 2023-12-02 17-51-03](https://github.com/KRIISHSHARMA/AWS/assets/86760658/1d1e3352-8c71-4714-91f4-b94a25168230)

- to see pods used by kubectl
![Screenshot from 2023-12-02 17-58-35](https://github.com/KRIISHSHARMA/AWS/assets/86760658/4621853e-23ea-4d95-be42-986136776895)

- autoscaler used by eks
![Screenshot from 2023-12-02 18-00-51](https://github.com/KRIISHSHARMA/AWS/assets/86760658/e926f3b6-ec65-43a1-854d-6c809c6680f4)

- can scale it 
![Screenshot from 2023-12-02 18-03-17](https://github.com/KRIISHSHARMA/AWS/assets/86760658/533bd710-6456-47ed-8235-266d641d31a9)

- install matrix server , will continue to moniter the cpu matrix ,without this will not show how much resources are utilised 
``` bash
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
```

- creating php-apache autoscaling yaml file for horizontal pod autoscaling
  ``` bash
  apiVersion: apps/v1
  kind: Deployment
  metadata:
    name: php-apache
  spec:
    selector:
      matchLabels:
        run: php-apache
    template:
      metadata:
        labels:
          run: php-apache
      spec:
        containers:
        - name: php-apache
          image: registry.k8s.io/hpa-example
          ports:
          - containerPort: 80
          resources:
            limits:
              cpu: 500m
            requests:
              cpu: 200m
  ---
  apiVersion: v1
  kind: Service
  metadata:
    name: php-apache
    labels:
      run: php-apache
  spec:
    ports:
    - port: 80
    selector:
      run: php-apache
  ---
  
  apiVersion: autoscaling/v1
  kind: HorizontalPodAutoscaler
  metadata:
    name: php-apache
    namespace: default
  spec:
    scaleTargetRef:
       apiVersion: apps/v1
       kind: Deployment
       name: php-apache
    minReplicas: 1
    maxReplicas: 10
    targetCPUUtilizationPercentage: 50
  ```

```  bash
nano hpa.yaml
```
- deploying
  ``` bash
  kubectl apply -f hpa.yaml
  ```
![Screenshot from 2023-12-02 18-46-22](https://github.com/KRIISHSHARMA/AWS/assets/86760658/95757273-91db-4065-9265-fbebcbe59cc2)
![Screenshot from 2023-12-02 19-07-14](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a99730d8-96b4-4915-b27e-53264933f50a)

- artificial load
  ``` bash
  kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"
  ```

- creating a load balancer type service 
![Screenshot from 2023-12-02 19-20-07](https://github.com/KRIISHSHARMA/AWS/assets/86760658/a815b33d-e2e0-4ade-b6e4-da263e14ad14)
- https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

- creating nodeport service
  ![Screenshot from 2023-12-02 19-26-13](https://github.com/KRIISHSHARMA/AWS/assets/86760658/57ca24cb-0985-4df1-89b0-14e87e1269df)
![Screenshot from 2023-12-02 19-34-42](https://github.com/KRIISHSHARMA/AWS/assets/86760658/4da03506-cefb-4e4e-9b32-e81743bb4d6e)

![Screenshot from 2023-12-02 19-33-13](https://github.com/KRIISHSHARMA/AWS/assets/86760658/63a123b8-95fb-46ce-a57d-b9098359d1ef)


## EKS 
![Screenshot from 2023-12-02 16-04-58](https://github.com/KRIISHSHARMA/AWS/assets/86760658/86c01036-bc68-4035-a38f-21a253b80f20)
![Screenshot from 2023-12-02 16-08-06](https://github.com/KRIISHSHARMA/AWS/assets/86760658/694af61d-a154-461c-a15c-33cf94787fe4)

- **BY KRIISH SHARMA**














 

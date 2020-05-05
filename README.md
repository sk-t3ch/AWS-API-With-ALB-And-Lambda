# T3chFlicks - API with ALB and Lambda
A Hello World example of an API created using 
AWS Lambda and Application Load Balancer. 
See the accompanying blog post [here](https://medium.com/p/b32b126bbddc).

### Usage
```
$ curl loadb-LoadB-R7RVQD09YC9O-1401336014.eu-west-1.elb.amazonaws.com
Hello World!
```

### Architecture
![Architecture](./architecture.png)

### Setup
1. Deploy VPC
    * `aws cloudformation create-stack --stack-name vpc --template-body file://aws/vpc.yml --capabilities CAPABILITY_NAMED_IAM`
    * tutorial for VPC can be found [here](insert_medium_link)
1. Deploy Service
    * `aws cloudformation create-stack --stack-name service --template-body file://aws/service.yml --capabilities CAPABILITY_NAMED_IAM`

---

This project was created by [T3chFlicks](https://t3chflicks.org) a tech focused education and service company.

---


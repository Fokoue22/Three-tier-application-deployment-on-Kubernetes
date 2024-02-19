# Threetier-application-deployment-on-Kubernetes

![alt text](three-app-deployment-image.gif)

# what do you mean by three tier ?
It’s actually a division of your system in 3 parts

## 1. Presentation Layer (Tier 1):
What you you see when you open your website is called the presentation layer basically it is the layer that users interact directly

## 2. Logical Layer (Tier 2):
Imagine this layer as the brain behind the scenes. It takes the information you provide through the user interface and processes it according to the rules of the system. If it’s a shopping website, for instance, this layer figures out things like the total price of your items, applies discounts, and checks if everything is in stock

## 3. Data Layer (Tier 3):
This is where the data is stored and retrieved. It’s like the memory of the system.
Data could be stored in databases, files, or any other data storage systems.
The data layer is responsible for managing and storing information that the system needs.

# Completion Steps →

### Phase 1 →Setup base EC2 , IAM user and Basic tools on EC2
### Phase 2 →Built frontend and backend images
### Phase 3 → Kubernetes
### Phase 4 →Setup Application Load balancer and ingress
### Phase 5 →Destroy Everything


# Phase 1 →Setup base EC2 , IAM user and Basic tools on EC2
## Step 1. Create an IAM user
Don't forget to attach `administratorAcces` policies directly to your iam user

![alt text](iam-creation.png)

`Then click on your IAM user` → 
Security credentials scroll down to access keys and create an access keys. Choose aws cli from the options listed

![alt text](create-accesskeys.png)


## Step 2. launching a base EC2 where we do all work →
Open your aws console and navigate to ec2 and click on launch ec2 `select ubuntu as your machine image`

![alt text](launch-ec2.png)
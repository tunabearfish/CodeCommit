## 📝 Prerequisites
  - Have an active AWS account
  - IAM User or Role
  - AWS CLI
  - SSH Key Pair(Optional)
  - GIT client
  - Access to the internet
  - GIT Credential Helper Configuration(optional)
  - AWS Region Selection

## 🛠 Set up

### 1. Open CodeCommit Console
![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/f38a5dbe-adf0-454b-a00e-7ed6a16e619d)
  In the AWS Management Console, navigate to the CodeCommit service by either searching for "CodeCommit" in the services search bar or locating it under the "Developer Tools" section
  
### 2. Create a New Repository
  ![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/5f1d986d-6d90-45ae-8e3f-6a7271351960)

  In the CodeCommit dashboard, click the "Create repository" button
### 3. Configure Repository Settings:
![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/a4e7645d-6946-47cd-bd10-abb88dfe2dcb)

  Fill out the repository creation form with the following details:
  Repository name: Choose a unique name for your repository.
  Description: Optionally, provide a description for your repository.

  For this example - I named my Repository: my-nodejs-app

### 5. Create Repository

### 6. Upload a file
![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/7d7254ed-c005-4e40-a2e5-1318d44a9b3e)


  In this example I will upload a index.html file
  For author: I used Steven
  Email address : steven@example.com
  Commit message - optional

  Click on Commit

### 6.Set up Notifcations
![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/88eaab42-3336-4da6-89a8-17fa5c8297f1)
  Back on the dashboard of our repository, move to settings and click on notifications

  Click on Create Notification

![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/84910b8c-90ac-4701-8b01-711a223debd5)

  In this exmaple I named this rule DemoNotificationRule
  For Events that trigger notifications: I select All

![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/6d4155bb-1641-461f-918f-3b50227d5d00)

  For Target, I clicked on Create Target

  My type is SNS topic
  I named it codecommit-lab

  Hit Create then hit submit



### 7. Triggers
Back in our repository settings, we can select our code and then select Triggers
![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/09b05e2e-2799-4204-abeb-6c2d2684e911)
  Click on Create Trigger
![image](https://github.com/tunabearfish/CodeCommit/assets/65553627/7983264f-c300-49cf-9d1e-d148f5474859)
  In this example, I named my Trigger name: DemoTrigger

  Events: push to existing branch
  Branch names(optional) - main

  Service Details: I chose Amazon SNS
  SNS topic: We can use the same one from our notifications(codecommit-lab)

  Hit Create trigger







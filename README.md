# Automating the Provisioning of Cloud Infrastructures using IaC and Cloud Services

## Architecture

![Architecture](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/Architecture.png?raw=true)

## Tasks
* Automate the provisioning of cloud infrastructures

By using the console:
1. Create IaC Templates ([IaC-template-1.yaml](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/code/iac-template-1.yaml) and [IaC-template-2.yaml](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/code/iac-template-2.yaml))

2. Create a CodeCommit Repository
![CodeCommit](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodeCommit.png?raw=true)

3. Push the files into CodeCommit Repository
```sh
# Clone the repo
git clone https://<CodeCommit Repo>/Infra-Repo

# Change the directory
cd Infra-Repo

# Add file: IaC Template 1

# Push to the repository
git add .
git commit -m "First Infra"
git push
```

4. Create a CodePipeline

a. Set-up the CodePipeline
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%20a-1.png)
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%20a-2.png)

b. Create an IAM role for CloudFormation
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%20b.png)

c. Add deploy stage
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%20c-1.png)
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%20c-2.png)

d. Create the pipeline
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%20d.png)

5. Check the pipeline if it's working correctly

a. CodePipeline
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%205-a.png)

b. CloudFormation
![](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/CodePipeline%205-b.png)

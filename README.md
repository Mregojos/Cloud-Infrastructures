# Automating Cloud Infrastructures with IaC and Cloud Services

## Architecture

![Architecture](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/images/Architecture.png?raw=true)

## Tasks
* Automate the provisioning of cloud infrastructures

By using the console:
1. Create IaC Templates ([iac-template-1.yaml](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/code/iac-template-1.yaml) and [iac-template-2.yaml](https://github.com/Mregojos/Cloud-Infrastructures/blob/main/code/iac-template-2.yaml))

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

4. 


# Solutions for Exercises-05-Cloud-IaaS-Basics

## Exercise 0

```bash
# Navigate to the working directory.
cd Repositories

# Cloning.
git clone https://gitlab.com/twn-devops-bootcamp/latest/05-cloud/cloud-basics-exercises.git

# Deleting .git folder.
rm -rf cloud-basics-exercises/.git

# Renaming the folder, because I want to save it to my GitHub repository with a different name.
mv cloud-basics-exercises TWN-DevOps-Bootcamp-Exercises-05-Cloud-IaaS-Basics
cd TWN-DevOps-Bootcamp-Exercises-05-Cloud-IaaS-Basics

git init
git status

# Commit & push.
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/ImreBodnar/TWN-DevOps-Bootcamp-Exercises-05-Cloud-IaaS-Basics.git
git push -u origin main
```

## Exercise 1

```bash
# Navigate to the working directory.
cd Repositories/TWN-DevOps-Bootcamp-Exercises-05-Cloud-IaaS-Basics/app

# Packaging the app.
npm pack
```

## Exercise 2

```bash
# Creating a new SSH key-pair for my new droplet...
ssh-keygen
cat ~/.ssh/id_ed25519.pub
# After I created a new droplet on DigitalOcean by using my new SSH keypair...
ssh -i ~/.ssh/id_ed25519 root@139.59.211.243
```

## Exercise 3

```bash
ssh -i ~/.ssh/id_ed25519 root@139.59.211.243

sudo apt update
sudo apt install -y nodejs npm
nodejs --version
npm --version
```

## Exercise 4

```bash
# Doing this without ssh-ing into the droplet...
scp bootcamp-node-project-1.0.0.tgz root@139.59.211.243:/root
```

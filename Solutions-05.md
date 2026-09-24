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

<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Connect a GitHub Repo with AWS

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-devops-github)

**Author:** Nii OB  
**Email:** davidniiamui@gmail.com

---

## Connect a GitHub Repo with AWS

![Image](http://learn.nextwork.org/genuine_navy_mysterious_monkey/uploads/aws-devops-github_dd9d254e)

---

## Introducing Today's Project!

Today, I'll set up a Git repository for the web app's code. This is project TWO in the 7 Day DevOps Challenge.
By the end of the project, the code I'll write for the Java web app will be stored securely in GitHub.

### Key tools and concepts

Services I used were GitHub, Amazon EC2, (development instance), key pairs and VSCode.
Key concepts I learnt include setting up a Git repository, the difference between Git and GitHub and the commands for staging, saving & pushing changes to my code.

### Project reflection

This project took me approximately 2 hours, including demo and troubleshooting time.
It was most rewarding to see the README tie everything together.
It was most challenging to learn all the different Git commands (add, commit, stage, origin, remote)

I did this project today to learn more about Git and GitHub - AND because  it's Day TWO of the 7 Day DevOps challenge!
I'm excited to have a repository that stores my web app's source code.

This project is part two of a series of DevOps projects where I'm building a CI/CD pipeline! I'll be working on the next project tomorrow.

---

## Git and GitHub

Git is a version control system that tracks changes made in code. This is incredibly helpful for collaboration, as you can see WHO made WHAT change in the code.
I installed Git using the commands 'sudo dnf update -y and
sudo dnf install git -y'.

GitHub is a platform that lets us store, share, and collaborate on our code.
It's called GitHub because it uses Git as the tool for version control and many more features.
I'm using GitHub in this project to store the web app's code.

![Image](http://learn.nextwork.org/genuine_navy_mysterious_monkey/uploads/aws-devops-github_efaadbf7)

---

## My local repository

A Git repository is like an online folder you can use to store your web app's code and all the versions of that code. 
It is the go-to place for all the code, updates and changes related to a specific project.

'git init' is a command that initializes git in our local repository.
I ran 'git init' in the web app project folder, which tells the terminal that I want to start tracking changes locally.

After running git init, the response from the terminal was that I initialized Git, and by default I'm using the 'main' branch.
A branch in Git is a copy of your code where you can make changes safely. It won’t affect the main code until you merge it.

![Image](http://learn.nextwork.org/genuine_navy_mysterious_monkey/uploads/aws-devops-github_7bf21bae)

---

## To push local changes to GitHub, I ran three commands

### git add

The first command I ran was 'git add .', which adds the changes to a staging area.
A staging area in Git is like the place to review all changes made to the code, so you can decide what changes you'd like to save in a commit.

### git commit

The second command I ran was 'git commit', which is the command for saving the changes in the staging area.
Using '-m' means I'm also leaving a message for that commit, e.g. "made changes to index.jsp"

### git push

The 3rd command I ran was 'git push -u origin master', to push saved code changes to the remote origin. The -u flag sets it as the default upstream, so future pushes only need git push, and Git will know where to send the changes.

---

## Authentication

When I committed changes to GitHub, Git asks for my credentials because it needs to authenticate me before letting me make code changes to the GitHub repository.
It needs to do this to know that I have the right to change the code.

### Local Git identity

Git needs my name and email because it is a version control system, which means it tracks who makes changes in a project. This info is added to each commit, helping with collaboration and version history.

Running git log showed me that by default, Git is saving my code changes to a username called 'EC2 Default User' instead of my actual name and details.

![Image](http://learn.nextwork.org/genuine_navy_mysterious_monkey/uploads/aws-devops-github_9a27ee3b)

---

## GitHub tokens

GitHub authentication failed when I entered my password because password authentication was already removed in 2021.
There are too many security risks associated with entering a password over the terminal to GitHub, so more secure ways are available.

A GitHub token is like a temporary password that grants access to your GitHub account.
I'm using one in this project because it lets me safely authenticate to my GitHub repository while in my EC2 instance.

I could set up a GitHub token by visiting the Developer settings in GitHub, and I set one up that expired in about 10 days, and only allow permissions to repositories.

![Image](http://learn.nextwork.org/genuine_navy_mysterious_monkey/uploads/aws-devops-github_fa11169d)

---

## Making changes again

I wanted to see Git working in action, so I made another change to my index.jsp file.
I couldn't see the changes in my GitHub repo initially because I hadn't added, committed, or pushed those changes.

I finally saw the changes in my GitHub repo after running the same 3 commands and then refreshing index.jsp in my GitHub repository.


![Image](http://learn.nextwork.org/genuine_navy_mysterious_monkey/uploads/aws-devops-github_6becb2bc)

---

## Setting up a READMe file

---

---

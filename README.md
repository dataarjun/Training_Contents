# The Software Development Life Cycle

![](/images/03BAD6B2-3427-4242-817E-78983C06DEB4.jpeg)
## Learning Objectives

#### Conceptual
- Explain what SDLC is and why we use it
- Provide a general overview of what "Agile" means and compare it to Waterfall
- Explain what SCRUM is, and how it relates to agile.
- Describe the process of requirements gathering.
- Explain what a user story is, and what specific points it should include.
- Describe what the backlog is, and how it gets prioritized.
- Describe what a sprint is, and the major parts of a sprint cycle.
- Describe what a wireframe is, and what it accomplishes.
- Describe the structure of a daily scrum meeting.
- Explain what Pivotal Tracker is and what problem it solves

#### Mechanical
- Distill project requirements into user stories.
- Prioritize a backlog, and plan a sprint.
- Wireframe intended application flow before starting work.

## SDLC
- Describes a process for planning, creating, testing, and deploying software
- Process is really important because without one, it's very easy to fall into the following traps:
    + Poor collaboration/communication among team members
    + Poor (or no) estimation of time to complete project
    + Missing or poorly planned features or functionality
    + Poor or no proritization of features
    + Inability to add (or remove) members from the project
    + Scope creep
    + <strike>Software that doesn't actually meet the needs of users</strike>
- Generally the process involves the following steps:
    + Requirements gathering
    + Design
    + Development
    + Testing
    + Bug fixing
    + Deployment

## Agile vs. Waterfall Methodologies

#### Waterfall
- Follows a step by step process where each step waits on the previous one
- Design and develop all features of an application in one fell swoop
- **Advantages**:
    + Clearly defines scope of project
    + Keeps clients and company on the same page, this is what the end result looks like
    + Documentation is potentially easier, allowing newer entrants to get up to speed quickly
- **Disadvantages**:
    + Slow
    + Doesn't adapt well to change
    + Doesn't handle user feedback well
    + Can drown in paperwork and bureaucracy

#### Agile
- Built to adapt to change
- Getting to MVP is the goal
- Relies on tight feedback loops
- <strike>Experimentation is good, as long as we measure the results</strike>
- <strike>Highly analytical</strike>
- **Advantages**:
    + Rapid iteration
    + Built to adapt to change
    + Allows us to catch bugs during the development cycle and not just at the end
    + Provides channels for user feedback to be integrated into future iterations
- **Disadvantages**:
    + Deliverables are constantly changing
    + Bugs can be more common as rapid iteration yields unexpected results
    + Documentation is frequently poor because requirements are changing all the time

## Agile Subsets

#### Kanban

- Kanban is about improving workflow, finding bottlenecks, inefficiencies, other problems
- Implemented by Toyota in the 1940's
- Kanban recommends moving the pieces of work through a "board" of different stages, notably
- Allows us to: 
 * Visualize the work flow - Making the work visible—along with blockers, bottlenecks and queues—instantly leads to increased communication and collaboration
 * Limit the WIP (Work in progress) - You can avoid problems caused by task switching and reduce the need to constantly reprioritize items
 * Focus on the flow - leads to culture of continuous improvements, any potential problems can be seen before it's too late

> Using our development pipeline as an example: if the testers are only able to test 5 features per week whereas the developers and analysts have the capacity to produce 10 features per week, the throughput of the pipeline as a whole will only be 5 features per week because the testers are acting as a bottleneck.

> If the analysts and developers aren't aware that the testers are the bottleneck, then a backlog of work will begin to pile up in front of the testers.

> The effect is that lead times go up. And, like warehouse stock, work sitting in the pipeline ties up investment, creates distance from the market, and drops in value as time goes by.

> Inevitably, quality suffers. To keep up, the testers start to cut corners. The resulting bugs released into production cause problems for the users and waste future pipeline capacity.

> If, on the other hand, we knew where the bottleneck was, we could redeploy resources to help relieve it. For example, the analysts could help with testing and the developers could work on test automation.

<img src="http://kanbanblog.com/explained/image/kanban-board-1.png">

<img src="http://kanbanblog.com/explained/image/kanban-board-2.png">

<img src="http://kanbanblog.com/explained/image/kanban-board-3.png">

#### Scrum
- Scrum is a subset of Agile, it's an "iterative" and "incremental" software development methodology for managing product development
- Scrum recommends breaking things into small pieces of work, and timeboxing our development cycles
- Scrum sets roles like: 
 * Product Owner (defines product vision, priorities, accepts & rejects work performed)
 * Team (implements product)
 * Scrum Master (improves process, sets sprint duration and removes impediments)
- Scrum process: 
 1. Create a product backlog (wishlist)
 2. Sprint planning, what will be in the current sprint? 
 3. Sprint/development (typically 2-4 weeks)
  - Meet daily for scrum meetings, organized by the scrum master
 4. Sprint review - Review the work done with the product owner 
 5. Sprint retrospective - what worked, what didn't about the process
 6. Ship and repeat 
- What is a scrum meeting/standup?
 + When does it happen?
   - Every morning for 15 min
 + What is the structure?
    1. What did I accomplish yesterday? 
    2. What will I work on today? 
    3. What impedes me or is blocking my progress? 
 + What is the point?
- Longer term plans
 + Release plan - Typically requires multiple sprints
 + Product roadmap

#### User Stories

- A user story is a very high-level definition of a requirement, containing just enough information so that the developers can produce a reasonable estimate of the effort to implement it
- Keep user stories slim and high level
- Anyone is able to write it
- Examples: 
 * Students can purchase monthly parking passes online.
 * Parking passes can be paid via credit cards.
 * Parking passes can be paid via PayPal.
 * Professors can input student marks.
 * Students can obtain their current seminar schedule.
 * Students can order official transcripts.
 * Students can only enroll in seminars for which they have prerequisites.
- Assign points based on how large the tasks are relative to each other, don't focus on the details
- Epic stories should be broken down into smaller ones 

## Class Exercise 

**Pair Exercise - 15 min**

Using index cards, write 5-10 user stories for a Craigslist website clone. Assign a point value from 1-3 to them for use later.

#### Sprints
- Sprints are development cycles for Scrum
- Use point systems to load with the amount of stories for each sprint
- Scrum requires a working product increment during each sprint. The product itself doesn't have to be shippable, but the increment to the product should be solid and functional

#### Retros
- How can we make our process better next time? How can we continually improve?

## Class Exercise 

**20 min**

Using Pivotal Tracker (https://www.pivotaltracker.com), add the user stories from the previous exercise into the backlog, and prioritize them. 


# GIT and DEVOPS Training

## how to create ssh key for github

>
$ ls -al ~/.ssh
# Lists the files in your .ssh directory, if they exist
generate ssh key github

>
$ ssh-keygen -t ed25519-sk -C "your_email@example.com"

### add ssh keys to github
>
    1. ssh-keygen -o -t rsa -C "your_email@example.com"
    2. Press return for each option
    3. cat ~/.ssh/id_rsa.pub               # This is your public key file ends with .pub
    4. Copy the entire cat's output on "Settings - SSH and GPG keys - New SSH key" on GitHub
    5. 




## Ensure you have a Github account created.
### Github Account Creation Steps:
1. Open https://github.com in a web browser, and then select Sign up.
2. Enter your email address.
3. Create a password for your new GitHub account, and Enter a username, too. Next, choose whether you want to receive updates and announcements via email, and then select Continue.
4. Verify your account by solving a puzzle. Select the Start Puzzle button to do so, and then follow the prompts.
5. After you verify your account, select the Create account button.
6. Next, GitHub sends a launch code to your email address. Type that launch code in the Enter code dialog, and then press Enter.
7. GitHub asks you some questions to help tailor your experience. Choose the answers that apply to you in the following dialogs:
8. On the Where teams collaborate and ship screen, you can choose whether you want to use the Free account or the Team account. To choose the Free account, select the Skip personalization button.

## Next Steps

### Create and use a repository

> Open a project from a GitHub repo:

    Visual Studio makes it easy to open a project from a repo. You can do so when you start Visual Studio, or you can do so directly from within the Visual Studio IDE.

    1 Open Visual Studio.
    2 On the start window, select Clone a repository.
    3 Enter or type the repository location, and then select the Clone button.
    4 You might be asked for your user sign-in information in the Git User Information dialog box. You can either add   your information or edit the default information it provides.
    5 Select Save to add the info to your global .gitconfig file. (Or, you can select Cancel if you>d like to add the info later.)
> FOr Visual Steps follow the below link : https://visualstudio.microsoft.com/vs/github/


# SSH Keys for GitHub

### Why Use an SSH Key?
**********************************************************************************************************************************************
>
    When working with a GitHub repository, you'll often need to identify yourself to GitHub using your username and password. An SSH key is an alternate way to identify yourself that doesn't require you to enter you username and password every time.

    SSH keys come in pairs, a public key that gets shared with services like GitHub, and a private key that is stored only on your computer. If the keys match, you're granted access.

    The cryptography behind SSH keys ensures that no one can reverse engineer your private key from the public one.
Generating an SSH key pair

1. The first step in using SSH authorization with GitHub is to generate your own key pair.

2. You might already have an SSH key pair on your machine. You can check to see if one exists by moving to your .ssh directory and listing the contents.

    $ cd ~/.ssh
    $ ls
If you see id_rsa.pub, you already have a key pair and don't need to create a new one.

3. If you don't see id_rsa.pub, use the following command to generate a new key pair. Make sure to replace your@email.com with your own email address.

    >
        $ ssh-keygen -o -t rsa -C "your@email.com"
(The -o option was added in 2014; if this command fails for you, just remove the -o and try again)

 When asked where to save the new key, hit enter to accept the default location.

    Generating public/private rsa key pair.
    
    Enter file in which to save the key (/Users/username/.ssh/id_rsa):
4. You will then be asked to provide an optional passphrase. This can be used to make your key even more secure, but for this lesson you can skip it by hitting enter twice.

Enter passphrase (empty for no passphrase):
Enter same passphrase again:
When the key generation is complete, you should see the following confirmation:

    Your identification has been saved in /Users/username/.ssh/id_rsa.
    Your public key has been saved in /Users/username/.ssh/id_rsa.pub.
 
- The key fingerprint is:

~~~
    01:0f:f4:3b:ca:85:d6:17:a1:7d:f0:68:9d:f0:a2:db your@email.com
    The key's randomart image is:
    +--[ RSA 2048]----+
    |                 |
    |                 |
    |        . E +    |
    |       . o = .   |
    |      . S =   o  |
    |       o.O . o   |
    |       o .+ .    |
    |      . o+..     |
    |       .+=o      |
+-----------------+
The random art image is an alternate way to match keys but we won't be needing this.

~~~~
5. Add your public key to GitHub
We now need to tell GitHub about your public key. Display the contents of your new public key file with cat:

    $ cat ~/.ssh/id_rsa.pub
The output should look something like this:

    ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEA879BJGYlPTLIuc9/R5MYiN4yc/YiCLcdBpSdzgK9Dt0Bkfe3rSz5cPm4wmehdE7GkVFXrBJ2YHqPLuM1yx1AUxIebpwlIl9f/aUHOts9eVnVh4NztPy0iSU/Sv0b2ODQQvcy2vYcujlorscl8JjAgfWsO3W4iGEe6QwBpVomcME8IU35v5VbylM9ORQa6wvZMVrPECBvwItTY8cPWH3MGZiK/74eHbSLKA4PY3gM4GHI450Nie16yggEg2aTQfWA1rry9JYWEoHS9pJ1dnLqZU3k/8OWgqJrilwSoC5rGjgp93iu0H8T6+mEHGRQe84Nk1y5lESSWIbn6P636Bl3uQ== your@email.com
   
    Copy the contents of the output to your clipboard.
    
6. Go to your github account and add the rsa key that you have generated following steps 1-5. Check the screenshot below .

![](/images/Adding_ssh_keys.PNG)


### *** Some important things to note if you are getting any errors

Make sure you are using ssh for your repository also

    git remote -v
    origin  git@github.com:eMahtab/reponame.git (fetch)
    origin  git@github.com:eMahtab/reponame.git (push)
    
>
Don't use https, if your remote is using https then it will keep asking for password, even If you have added the public key to Github and added private key to ssh-agent. Below will always ask for password



### Make changes to a file and push them to GitHub as commits

> 1. cd /your_project path
>    
     1. git add *
     2. git commit -m "Enter commit message here"
     3. git push -u origin "YYourBranchName"

### Open and merge a pull request





## Git Branching and Merging

### Create a new branch with git and manage branches

In your Github fork, you need to keep your master branch clean, by clean I mean without any changes, like that you can create at any time a branch from your master. Each time that you want to commit a bug or a feature, you need to create a branch for it, which will be a copy of your master branch.


1.  When you do a pull request on a branch, you can continue to work on another branch and make another pull request on this other branch.
    Before creating a new branch, pull the changes from upstream. Your master needs to be up to date.

   > $ git pull

2. Create the branch on your local machine and switch in this branch :

   > $ git checkout -b [name_of_your_new_branch]
3. Push the branch on github :

    > $ git push origin [name_of_your_new_branch] 
4. When you want to commit something in your branch, be sure to be in your branch. Add -u parameter to set-upstream.

    You can see all the branches created by using :

    > $ git branch -a 

    Which will show :

    * approval_messages
    master
    master_clean
5. Add a new remote for your branch :

    > $ git remote add [name_of_your_remote] [name_of_your_new_branch]
6. Push changes from your commit into your branch :

    > $ git push [name_of_your_new_remote] [url]
    OR 
    > $ git push -u  origin [name_of_your_new_remote]

7. Update your branch when the original branch from official repository has been updated :

    > $ git fetch [name_of_your_remote]

8. Then you need to apply to merge changes if your branch is derivated from develop you need to do :

    > $ git merge [name_of_your_remote]/develop

9. Delete a branch on your local filesystem :
    Ensure you have switched your barnch to main otherwise it may give error.
    > git switch main

    > $ git branch -d [name_of_your_new_branch] 
    Example: git branch -d  git-commands
    Output:  Deleted branch git-commands (was 601b25c).

10. To force the deletion of local branch on your filesystem :

    > $ git branch -D [name_of_your_new_branch]
    Delete the branch on github :

    > $ git push origin :[name_of_your_new_branch]
    The only difference is the: to say delete, you can do it too by using GitHub interface to remove branch: https://help.github.com/articles/deleting-unused-branches.

    If you want to change default branch, it>s so easy with GitHub, in your fork go into Admin and in the drop-down list default branch choose what you want.

    ### If you want create a new branch:

    > $ git branch <name_of_your_new_branch>


## In summary, if you want to contribute to a project, the simplest way is to:

    - Find a project you want to contribute to
    - Fork it
    - Clone it to your local system
    - Make a new branch
    - Make your changes
    - Push it back to your repo
    - Click the Compare & pull request button
    - Click Create pull request to open a new pull request



# We are learning to develop a claculator app

## CalculatorApp-In-Flask

### 💻 Tech Stack
### Front-End:
<img alt="HTML5" src="https://img.shields.io/badge/html5%20-%23E34F26.svg?&style=for-the-badge&logo=html5&logoColor=white"/>  <img alt="CSS3" src="https://img.shields.io/badge/css3%20-%231572B6.svg?&style=for-the-badge&logo=css3&logoColor=white"/> <img alt="JavaScript" src="https://img.shields.io/badge/javascript%20-%23323330.svg?&style=for-the-badge&logo=javascript&logoColor=%23F7DF1E"/> 
<img alt="BootStrap" src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white"/> 

### Back-End:
<img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/> <img alt="Flask" src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"/> 

## 🚀 Quick Start :


#### Step 1: Forking the repository :

To work on an open-source project, you will first need to make your copy of the repository. To do this, you should fork the repository and then clone it so that you have a local working copy.

Get your own Fork/Copy of repository by clicking `Fork` button right upper corner.<br><br>

#### Step 2: Clone the Forked Repository

After the repository is forked, you can now clone it so that you have a local working copy of the codebase.

To make your local copy of the repository follow the steps:
- Open the Command Prompt
- Type this command:
  
```bash
$ git clone https://github.com/<your-github-username>/CalculatorApp-In-Flask
```


#### Step 3: Creating a new branch (IMP)
This is one of the very important step that you should follow to contribute in Open Source. A branch helps to manage the workflow, isolate your code and does not creates a mess. To create a new branch:
  
```bash
$ git branch <name_of_branch>
$ git checkout -b <name_of_branch>
```

Keep your cloned repo upto date by pulling from upstream (this will also avoid any merge conflicts while committing new changes)
```bash
git pull origin main
```

#### Step 4: Setting up Project
##### For Flask:

**1. Create a Virtual Environment**

- *On macOS and Linux:*
  ```bash
    python -m venv calculator
  ```
- *Windows*
  ```bash
    py -m venv env
  ````

**2. Activate the Virtual Environment**
  - *On Windows*
    ```bash
    .\env\Scripts\activate
    ```
  - *On macOS and Linux:*
    ```bash
    source calculator/bin/activate
    ```

**3. Install dependencies using**
```bash
pip install -r requirements.txt
```

**4. Run server using**

```bash
python main.py

OR

flask run

```

**5.** Go to ` http://127.0.0.1:5000/` and enjoy the application.

#### Step 5: Contribute
Make relevant changes according to the issue that you were assigned on. Contribute in any way you feel like :)

#### Step 6: Commiting and Pushing
Once you have modified an existing file or added a new file to the project, you can add it to your local repository, which we can do with the git add command.

```bash
git add .
```
With our file staged, we’ll want to record the changes that we made to the repository with the git commit command.

The commit message is an important aspect of your code contribution; it helps the other contributors fully understand the change you have made, why you made it, and how significant it is.

```bash
git commit -m "useful commit message"
```

At this point you can use the git push command to push the changes to the current branch of your forked repository:

```bash
git push origin <branch-name>
```

#### Step 7: Create Pull Request
Now, you are ready to make a pull request to the original repository.

You should navigate to your forked repository, and press the "Compare & pull request" button on the page.

GitHub will alert you that you can merge the two branches because there is no competing code. You should add in a title, a comment, and then press the “Create pull request” button.


<br>
show some ❤️&nbsp; by giving the star to this repo







# CI/CD Process and Devops Process Floww

>   CI and CD stand for continuous integration and continuous delivery/continuous deployment. In very simple terms, CI  is a modern software development practice in which incremental code changes are made frequently and reliably. Automated build-and-test steps triggered by CI ensure that code changes being merged into the repository are reliable. The code is then delivered quickly and seamlessly as a part of the CD process. In the software world, the CI/CD pipeline refers to the automation that enables incremental code changes from developers’ desktops to be delivered quickly and reliably to production


![](/images/CI-CD_process.png)


## Deploying the calculator app in cloud:

### Clone an existing Git repo
    1. Get the clone URL for an Azure Repos Git repo
    2. Get the clone URL for a GitHub repo
    3. Clone an Azure Repos Git repo
    4. Clone a GitHub repo
    5.  Clone any Git repo
    6. Open a Visual Studio solution from a cloned repo

# CI/CD Pipeline for Machine Learning Project in Azure
Deploying a Flask Machine Learning Application on Azure App Services.

### Status

[![Python application test with Github Actions](https://github.com/marcoBrighterAI/flask-ml-azure-serverless/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/marcoBrighterAI/flask-ml-azure-serverless/actions/workflows/main.yml)

[![Build Status](https://dev.azure.com/marcopaspuel/Flask-ML-Deploy/_apis/build/status/marcoBrighterAI.flask-ml-azure-serverless?branchName=main)](https://dev.azure.com/marcopaspuel/Flask-ML-Deploy/_build/latest?definitionId=1&branchName=main)

### Introduction
This project builds a **Continuous Integration** pipeline using **GitHub Actions**, and a **Continuous Delivery** pipeline
using **Azure Pipelines** for a Machine Learning Application. The app is implemented in python using scikit-learn and the
flask module. **Azure App Services** is used to host the application. In this repo you will find all the code and configurations
necessary to implement CI/CD. The ML application is simple, however, it can be easily extended.

![pycharm1](images/project-architecture.png)

### Dependencies
- [Azure Account](https://portal.azure.com) 
- [Azure command line interface](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest) (Only if running locally)
- [Azure DevOps Account](https://dev.azure.com/) 

### Project Plan
To follow DevOps best practices, in the links bellow you will find a Kanban Trello board, and a spreadsheet
showing the project plan, project deliverables and project goals.

* [Trello board](https://trello.com/b/boMOaYDS/ci-cd-pipeline-for-machine-learning-project-in-azure)
* [Project plan spreadsheet](https://docs.google.com/spreadsheets/d/1YuwbRiXFODAtWOqejUCbbSH1ag5XcuXN_TyVgkzjHNE/edit?usp=sharing)

### Getting Started

1. Fork this repository
2. Log into the [Azure Portal](https://portal.azure.com) 
3. Launch Azure Cloud Shell 

### Instructions
To run this project in the Azure Cloud Shell, follow the steps bellow. The same steps apply when running locally, however,
you would need to log into your Azure Account from the terminal first.

- [1. Clone the forked repo in Azure Cloud Shell](#1-clone-the-forked-repo-in-azure-cloud-shell)
- [2. Create virtual environment and source](#2-create-virtual-environment-and-source)
- [3. Deploy your app in Azure Cloud](#3-deploy-your-app-in-azure-cloud)
- [4. Verify Machine Learning predictions works](#4-verify-machine-learning-predictions-works)
- [5. Verify Continuous Integration by changing app.py](#5-verify-continuous-integration-by-changing-apppy)
- [6. Create a Webapp in Azure App Services](#6-create-a-webapp-in-azure-app-services)
- [7. Create an Azure DevOps Project and connect to Azure](#7-create-an-azure-devops-project-and-connect-to-azure)
- [8. Create a Python Pipeline with GitHub Integration](#8-create-a-python-pipeline-with-github-integration)
- [9. Verify Continuous Delivery by changing app.py](#9-verify-continuous-delivery-by-changing-apppy)
- [10. Verify Machine Learning Prediction in Azure Apps](#10-verify-machine-learning-prediction-in-azure-apps)
- [11. Load test the application using Locust](#11-load-test-the-application-using-locust)


#### 1. Clone the forked repo in Azure Cloud Shell
``` bash 
    git clone git@github.com:dataarjun/calculator-app.git
    cd calculator-app/
    ls
```
![pycharm1](images/git-clone-output.png)

Note:  You may need to follow this YouTube video guide on how to [setup SSH keys and configure Azure Cloud Shell with Github](https://www.youtube.com/watch?v=3vtBAfPjQus).

#### 2. Create virtual environment and source
``` bash 
    make setup
    source ~/.calculator-app/bin/activate
```
#### 3. Deploy your app in Azure Cloud 
To start the app run the following commands:
``` bash 
    make all
    python main.py
```
![pycharm2](images/make-all-output.png)

After running both commands you should see an output like the screenshot bellow.

![pycharm3](images/python-app-output.png)

Now you can open the *Web preview* by clicking in the icon depicted with the red dot in the image above and set the port to `5000`.
A new window will open, and you should see you web app running. See image bellow.
![pycharm4](images/web-app-running.png)

#### 4. Verify Machine Learning predictions works
First open a new Azure Cloud Shell then run the commands bellow.
``` bash 
    cd calculator-app/
    ./make_predict.sh
```
The model should predict the output depicted bellow.

![pycharm5](images/prediction-output.png)

#### 5. Verify Continuous Integration by changing app.py
To verify that the Continuous Integration is working you can open the editor in Azure Cloud Shell and change the welcome
message in the [main.py](main.py) script (line 25). Then commit and push your changes. 

![pycharm6](images/change-welcome-message.png)

Now you can you open your GitHub repo and go to the *Actions* section. You will see that a new pipeline has been triggered.
The pipeline will test your changes and make sure that the code is in a deployable state. See image bellow.

![pycharm7](images/github-actions.png)

#### 6. Create a Webapp in Azure App Services
##### 6.1. Create a Resource Group
``` bash
    az group create --name "RESOURCE_GROUP_NAME" --location "LOCATION" --tags udacity=udacity-project2
```
##### 6.2. Set the default resource group and region for subsequent commands
``` bash
    az configure --defaults group="RESOURCE_GROUP_NAME" location="LOCATION"
```
##### 6.3. Run the following command to create and deploy the App Service app. Replace <your_app_name> 
with a unique name that becomes the URL, http://<your_app_name>.azurewebsites.net.
``` bash
    az webapp up --name <your_app_name> --logs --launch-browser

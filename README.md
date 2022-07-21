# GIT and DEVOPS Training

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
    python3 -m venv env
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
    source env/bin/activate
    ```

**3. Install dependencies using**
```bash
pip install -r requirements.txt
```

**4. Run server using**

```bash
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

![alt text]('/images/CI-CD_process.png')

# GitWorkshop_11thSep2022

This workshop can be divided into 2 parts:

1. Basic Training on Git and GitHub (Conceptual Understanding and Basic Commands)
2. How is Git and GitHub relevant to the students of IIT?

# BASIC TRAINING ON GIT AND GITHUB

The basic commands on git and github can be read from the following blog post: 
[Basic Commands On Git and GitHub](https://jahid1030.medium.com/basic-git-commands-every-developer-should-know-git-github-1e07d081af29) - *author: Abdullah Al Jahid (bsse1030@iit.du.ac.bd)*

# How is Git and GitHub relevant to the students of IIT?

From IIT’s perspective, students write 2 kinds of code namely - structured and object oriented.
Generally, all the structured codes can be stored in a single repository. But, one can surely keep them in different repositories. However, here we will discuss how to store all the codes in a single repository.

## Structured Codes

**Step 1:** Create a new directory/folder. You can name it as you want. I am naming it as FirstYear_Codes.

**Step 2:** Initialize a git repository inside that folder. Initializing a git repository means that from now onwards all the changes in this folder will be tracked by git.

```bash
$ git init
```

![image](https://user-images.githubusercontent.com/46520621/190827746-caeca7ff-aa43-4331-a068-ac06f693408c.png)


*Figure 1: Creating Git Repository*

The .git folder will be created. Keep in mind that .git is a hidden folder. So to see it, you need to toggle the hidden items option to true from view.

**Step 3:** Copy all of your structured codes in this directory. Then check the git status.

```bash
$ git status
```

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled.png)

*Figure 2: Checking Status*

You will find that all the copied files will be shown as untracked files.

**Step 4:** Stage all the files. Only the staged files will be prepared to be committed. Then check the status to see for yourself whether the files are staged.

```bash
$ git add .
$ git status
```

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%201.png)

*Figure 3: Staging Files*

**Step 5:** Commit the changes by writing an appropriate message.

```bash
$ git commit -m "code 1, 2 and 3 added"
```

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%202.png)

*Figure 4: Committing Changes*

Now, the changes have been saved to the local git repository. But, we want more than this, right? We want to store it in the cloud so that we can access it from anywhere.

**Step 6:** Click the add button. Then, click *New Repository* to create the github repository.

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%203.png)

*Figure 5: Creating Remote Repository (1)*

**Step 7:** Select an appropriate name and create the repository, an optional description and set the visibility to public to let everyone on the internet see this repository.

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%204.png)

*Figure 6: Creating Remote Repository (2)*

**Step 8:** Copy the following git command.

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%205.png)

*Figure 6: Linking Remote Repository with Local Repository (1)*

**Step 9:** Paste the copied command in the git bash.

```bash
$ git remote add origin https://github.com/ahmedryanfaiyaz/FirstYear_Codes.git
```

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%206.png)

*Figure 6: Linking Remote Repository with Local Repository (2)*

Now, your local repository is connected with your remote repository in the cloud.

**Step 10:** Push your local git changes to remote repository.

```bash
$ git push --all
```

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%207.png)

*Figure 7: Pushing changes to the remote repository*

Then, go and refresh your remote repository in the browser. And you will find something like the following figure.

![Untitled](GitWorkshop_11thSep2022%20c465293a579644659f129f47a4b863b3/Untitled%208.png)

*Figure 8: Remote repository view*

**Now, what if you want to push more codes (like Code_4.cpp, Code_5.cpp, Code_6.cpp and Code_7.cpp)?**
Simply, follow the Steps 3,4,5 and 10.

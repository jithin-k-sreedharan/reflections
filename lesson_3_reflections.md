---
title: Lesson 3 - Using GitHub
author: Jithin K. Sreedharan
header-includes:
    \usepackage{fancyhdr}
    \pagestyle{fancy}
    \fancyhf{}
    \rhead{Jithin K. Sreedharan}
    \lhead{Lesson 2}
    \cfoot{\thepage}
---

<!-- # Using GitHub -->

* GitHub is a website that makes it easy to share an entire git repository with other people.
* The local git repository needs to be synced to the GitHub repository. GitHub uses the concept of remote repository (simply _remotes_), that's the repository in Github. One only needs to commit a branch (called push branch). All the commits under that branch (by tracing parents) are synced to the GitHub repository.
* Looks like Github clone (`git clone`) is not possible from local repository to the Github server.
* Adding a remote:
    - Go to [https://github.com/new](https://github.com/new). Create a new repository.
    - Add the GitHub repository as a remote to the local repository (here "reflections") in my computer
    ``` bash
    git remote # View current remotes
    git remote add <name> <URL>
    #"Name" is any name that one can use to refer to the remote repository.
    # If there is only one remote, standard name is "origin"
    # Copy the HTTPS URL, not SSH URL from the GitHub info.
    git remote add origin https://github.com/jithin-k-sreedharan/reflections.git
    git remote # To see the added remote
    git remote -v # To see the details of added remote, "v" for verbose
    git push origin master # git push <origin> <master>
    ```
* For making the GitHub repository not to ask for password each time we push, follow [this link](https://help.github.com/articles/caching-your-github-password-in-git/).
* Reflections: When would you want to use a remote repository rather than keeping all your work local?  
    - To keep safe all my code and data of a project in a cloud
    - To share and collaborate projects with other people
* Pulling from the remote to local repository
    ``` bash
    git pull origin master # git pull <remote_name> <branch_name>
    ```

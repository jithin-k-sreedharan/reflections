# Lesson 2: Using `git`

* To initialize a git repository: `git init`
* What happens when you initialize a repository? Why do you need to do it?   
    When I initialize a repository, it creates the `.git` folder and its standard subfolders. Now it's ready for the first commit.
* Git related directories: Working directory -> Staging directory -> Repository.   
    Staging directory work as an intermediate step before commit. Use `git add file1 file2 ` or just say `git add --all`.
* How is the staging area different from the working directory and the repository? What value do you think it offers?   
    Only the changes or files mentioned in the staging area are going to be included in the final commit. Suppose we have multiple files changed since last commit, and we wish to include only a few files for the next commit since they constitute a logical change. We then include only those subset of changed files in the staging area.
* Use `git reset file1` to remove file1 from the staging area.
* Commit message style guide: [http://udacity.github.io/git-styleguide/](http://udacity.github.io/git-styleguide/). Write in a imperative tone and end without period, for e.g., "Add PDF of file1" instead of "Added PDF of file1". 
* Use `git status` intermittently to see which files has been committed, which are untracked etc.
*

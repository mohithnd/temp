1. `git init` -> Powers your folder to be managed by Git and initializes a new empty repository. It also creates a .git folder that has all the relevant logic to manage versions of your project.

2. `Working Area` -> There can be a bunch of files that are not currently handled by Git. It means that changes done or to be done in those files are not managed by Git yet. A file which is in the working area is considered not to be in the staging area. When we do `git status` and we see a bunch of `untracked files`, then these are actually called to be in the working area.

3. `Staging Area` -> What all files are going to be part of the next version that we will create. This staging area is the place where Git knows what changes will be done from the last version to the next version.

4. `Repository Area` -> This area actually contains the details of all your previous registered versions. And the files in this area, Git already manages them and knows their version history.

5. `git add <file>` -> Moves a file from the working area to the staging area.

6. `git rm --cached <file>` -> Moves a file back from the staging area to the working area.

7. `Commit` -> A commit is a particular version of the project. It captures a snapshot of the project's staged changes and creates a version out of it.

8. `git commit` -> Registers staging changes to a commit.

9. `git log` -> List downs all the commits of the repository.

10. `git restore <file>` -> It removes all file changes from the staging area to be commited. This can be useful, if we did some dirty piece of code and now we do not want it. Instead od deleting every changes line by line, We can restore it or you can say resotre last clean version of the file.

11. `git restore --staged <file>` -> It removes file from staging area to working area.

12. `Diff Between git rm And git restore` -> If you want to move the whole file back to the untrackd state, then we do git rm, otherwise if we just want changes to be moved in working area or staging area then we do git restore.

13. `git diff commit1 commit2` -> Gices the difference of all file changes between two commits.

14. `git commit -a "<your commit message>"` -> If we want to avoid opening a text editor like vim/nano we can use this command.

15. `git remote` -> List down all the remote connection names.

16. `Remote Connection` -> It helps you to link two git respositories for uploading and donwloading changes from each other.

17. `git remote add <name of remote> <lingk of the remote>` -> This command helps us to add a new link to the remote repo and give a name to it.

18. `git remote rm <name of remote>` -> This command deletes a remote connection.

19. `git remote rename <oldname> <newname>` -> This command renames the remote connection.

Note: The name of the remote connection is always used to establish the communication between repos.

20. `git add <file1> <file2> <file3>` -> This command will add multiple file changes togehter in the staging area.

21. `git add .` -> This command will add all files from workign repo to staging area.

22. `git pull <remote name> <branch name>` -> Downloads latest changes from the branch of the mentioned remote in your local repo.

Merge conflics can occur if multiple people try to make changes to the same file, and then collaborate.

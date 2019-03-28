# Creating and Pushing local Git Repo to GitHub (new local repo => remote)
## NOTE: If you haven't already generated and added your SSH Key to GitHub, go here:
* https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account

1. Using Terminal, Bash or your favorite Git GUI tool
    * Create a repo on your local filesystem from within your desired working directory
    ``` 
    $ git init
    ```
2. Add all your local files to your new repo and commit them with a comment using the -m switch.
    ``` 
    $ git add --all
    $ git commit -m "initial checkin"
    ```
2. Log into GitHub and create a repository. Do not close the window, you will need info from the next screen.
3. From the resulting page in GitHub, copy the "push an existing repository from the command line" or set your GIT GUI tool to the remote repository URL
    * Adding the Remote origin to your local repo via SSH using your existing SSH Key.
    ```
    $ git remote add origin git@github.com:<USERNAME>/<REPO_NAME>.git
    ```
4. Next, your will want to PUSH your local git repo up to the server.
    ```
    $ git push -u origin master
    ```
5. Now your local repo should be available to you in the GitHub website. Interact with it accordingly.
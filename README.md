**CLI Helpers**

I spend a lot of time on the command line and these things help me do that.

dirfor  
Usage: `dirfor <process name>`  
Output: the current directories in use by the processes with the given name  

git-to-vim  
Usage: `git-to-vim` (from within a git repo)  
Will open all currently modified files in your repo in Vim.  

trash-git-st  
Usage: `trash-git-st` (from within a git repo)  
Removes all directories and files listed by `git st`. Helpful for cleaning up
untracked files after a commit.

git-save

Usage:
```
git save //saves a stash branch with your current changes
git save <new branch name> //saves a stash branch using your name with your current changes
git save clear //removes all stash branches
```

Save the current state of your changes to a new branch names STASH-<new branch
name>-<timestamp>. Used as a more visible replacement to `git stash`.

reporter
Usage:
```
reporter echo 'hey'
```

Reporter will send a notification via [Pushover](pushover.net) when the given
command has completed. Useful for leaving your desk during long-running
commands.

Required environment variables:
1) PUSHOVER_API_KEY: your app's API key
2) PUSHOVER_USER_KEY: the recipient's Pushover key

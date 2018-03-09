Quick Notes for use of git and github.

# List Config
To list configuration details,
```bash
	git config --list
```

# Set Config ( global ) 
To set configuration parameters globally ie. to use for all repositories.
```bash
	git config --global user.name "<username>"
	git config --global user.email "<email address>"
```
To set configuration parameters for a specific repository,
```
	git config user.name "<username>"
	git config user.email "<email address>"
```

# Get local copy
To get local copy of a repository from distributed server, 
```
git clone <github-url>
```

# Publish changes

There three phases in git.

## Staging area ( buffer )
`git add` command is used to add the modified or new files/folders to the staging area. Note that `git add` will not give any output
```
- git add <filename>
- git add .    # add current directory changes
- git add -A   # add all the directories. 
- git status
```

## Local Repo:
 `git commit` is used to add to local repository. While commiting the files, SHA-1 key will be generated for every commit.
```
- git commit  			# this will open an editor to give commit message
- git commit -m "reason"	# -m used to give commit message in CLI itself
- git status			# will give info about files are in statging area,local repo, remote repo
				# Untracked files - which are not yet added to staging
				# Changes to be committed - which are in staging area
- git log
```

## Remote Repo
`git push` is used to push the changes to the distributed repository.
```
- git push 
- git push -u origin master
```

To get remote repo details,
```
- git remote -v
```

To rename remote repo name,
```
- git remote rename origin destination
- git remote -v
```

## Some git repo stuff
To initialize git repo locally,
```
- git init 
```
To add remote repo for local repo,
```
- git remote add origin <url>
```
To push the current branch and set the remote as upstream,
```
- git push --set-upstream origin master
```
To pull the recent content from remote repo,
```
- git pull origin master
```
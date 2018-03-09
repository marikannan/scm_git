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

# Set Config ( specific repo ) 
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
- git commit
- git commit -m "reason"
- git status
- git log
```

## Remote Repo
`git push` is used to push the changes to the distributed repository.
```
git push
```

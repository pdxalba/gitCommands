git help <command>  eg log, commit, checkout   Pulls up documentation  C:\Program Files\Git\mingw64\share\doc\git-doc\

touch <filename> create a new file from the command line

git status
git add .  or git add <filename.
git commit -m "<comment>"   commits a new or changed file to git
git ls-files   Files currentlyS 	 tracked by git
rm <filename> remove file
git commit -am "<comment>"  If a file is already tracked by git, you can add and commit in 1 step
git log   log info on your commits

git restore --staged <filename>  If you've git added a file and you want to revert it
git checkout -- <filename> if you want to overwrite a local file

git log --oneline --graph --decorate --all   info on single line, graph of branching hierarchy, which commits are part of which branches, 
											 history of all branches in the repo
		Output would be :
			* e198373 (HEAD -> master) updates and backouts
			* 052605c express commit 2
			* 59d39b9 express commit
			* fdc8531 commit 2
			* ed858e8 1st commit


git config --global --list   List git's config entries

git config --global alias.hist "log --oneline --graph --decorate --all"   Creates an alias called hist (with the command after)
	then using git hist executes the same as everything that was defined in the alias
	
git mv <old filename> <new filename>   renames a file	(still need to commit after)
git rm <filename> removes a file from git   (still need to commit after)

git add -u If a file has been deleted (outside git) this stages it (then you need to commit to delete)

git diff   tells you what's changed since last commit
	can be used to compare different commits (if you include the commit details
git difftool  goes into each file and shows you the changes since last commit
	can be used to compare different commits (if you include the commit details
	
git branch   tells you what branch you are in 
git checkout -b <new branch name>  creates a new branch and switches to it
git checkout <branch name> Switches branch
git merge <branch name>  Merges that branch into the branch you're in
git branch -d <branch name>  delete branch
git branch -a   lists all the branches   (local, staging and remote)

git fetch   get latest changes from remote (non destructive - local changes aren't overwritten) could be a file or a branch
git merge   merge changes in to remote (for the branch you're in)
git pull    combines a fetch and merge (for the branch you're in)
git pull --all  does a pull for all the branches you're tracking
git pull --rebase  rewinds local branch,  brings in changes from github and then reapplies any changes on the local branch

git push -u origin <local branch name>  pushing a branch to remote for the 1st time
git push origin :<remote branch name>   deletes a branch from the remote repo.  Needs the ":" before the branch name

     
rm -rf <local repo>    forcefully removes the local repo
 

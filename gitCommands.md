git status
git add .  or git add <filename.
git commit -m "<comment>"   commits a new or changed file to git
git ls-files   Files currentlyS 	 tracked by git
rm <filename> remove file
git commit -am "<comment>"  If a file is already tracked by git, you can add and commit in 1 step
git log   log info on your commits

git restore --staged <filename>  If you've git added a file and you want to revert it
git checkout -- <filename> if you want to overwrite a local file

git help <command>  eg log, commit, checkout   Pulls up doccumentation

git log --oneline --graph --decorate --all   info on single line, graph of branching hierarchy, which commits are part of which branches, history of all branches in the repo
		Output would be :
			* e198373 (HEAD -> master) updates and backouts
			* 052605c express commit 2
			* 59d39b9 express commit
			* fdc8531 commit 2
			* ed858e8 1st commit


git config --global --list   List git's config entries

git config --global alias.hist "log --oneline --graph --decorate --all"   Creates an alias calleg hist (with the command after)
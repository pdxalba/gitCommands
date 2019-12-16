Branching 3 types ;
	Fast Forward - where no commits were done to the parent branch
	Automatic - where no conflicts between the feature branch and parent branch
	Conflict - where manual merge has to be done between the feature branch and parent branch (conflicts exist)
	
HEAD -  marker to define the last commit of the current branch
	
	
git tag -a <tagname> -m "<comment for tag>    eg git tag -a v1.0 -m "Release 1.0"  Creates tag details

git tag --list   displays list of tags
git show <tagname>  Way more info about the tage. eg date / time. Who did it and what it contains
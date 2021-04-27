Reverting

Reverting is a way to undo changes with git but without moving backwards.

To first view your git history to view any changes made on your current branch 
you will use the command "git log".

You can also use "git log --oneline" to view these changes in a condensed on line format.

If your output looks similar to this:

 875f31e (HEAD -> main) fourth commit
 483856a third commit
 2dd011d second commit
 bcabb84 first commit

Then we execute "git revert HEAD" a new commit will be made which essentially undoes the previous/
forth commit. This allows us to continue using the same branch and keep moving forward but still 
be able to make changes. 

You can also use "git reset" however this replaces the previous commit and pretends it didn't exist
which could cause problems and confusion later.

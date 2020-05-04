# git aliases

# Following "git config" used to set up an alias for each command

$ git config --global alias.ci commit
$ git config --global alias.st status
$ git config --global alias.co checkout
$ git config --global alias.br branch

# Example 01:

# This "git config" used to set up an alias for "commit" command

$ git config --global alias.ci commit

# If you want to commit a file, you can use "git ci -m"<message>" " instead "git commit -m"<message>" " command:

$ git ci -m"message"

# Result for this command is:

$ git ci -m"message"
[master 9bb7d7e] message
 1 file changed, 1 insertion(+)
 create mode 100644 git aliases.md
$ 

# Example 02:

# This "git config" used to set up an alias for "status" command

$ git config --global alias.st status

# If you want to commit a file, you can use "git st" instead "git status" command:

$ git st

# Result for this command is:

$ git st
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   git aliases.md

no changes added to commit (use "git add" and/or "git commit -a")
$

# When you didn't add anything to commit, this result will occur. 

# Example 03:

# This "git config" used to set up an alias for "checkout" command

$ git config --global alias.co checkout

# If you want to commit a file, you can use "git co master" instead "git checkout master" command:

$ git co master

# Result for this command is:

$ git co master
M	git aliases.md
Already on 'master'
Your branch is up to date with 'origin/master'.
$

# Example 03:

# This "git config" used to set up an alias for "branch" command

$ git config --global alias.br branch

# If you want to commit a file, you can use "git br" instead "git branch" command:

$ git br

# This is a job to view current branch in the code repository 

# Example 04:

# This "git config" used to set up an alias for "reset HEAD --" command

# For example, to correct the usability problem you encountered with unstaging a file, you can add your own unstage alias to Git:

$ git config --global alias.unstage 'reset HEAD --'

# It equals following two commands:

$ git unstage fileA
$ git reset HEAD -- fileA

# Result for this command is:

$ git config --global alias.unstage 'reset HEAD --'
$ git unstage
Unstaged changes after reset:
M	git aliases.md
$ 

# Example 05:

# This "git config" used to set up an alias for "last commit"

$ git config --global alias.last 'log -1 HEAD'

# If you want to check a last commit, you can use "git last" instead "git log -1 HEAD" command:

git last

# Result for this command is:

$ git last

commit 9bb7d7e4d1f214d17dd97cfced7606852b8d48e2 (HEAD -> master, origin/master, origin/HEAD, hello_world_, hello_world)
Author: John Doe <johndoe@example.com>
Date:   Mon May 4 08:06:43 2020 +0530

    draft
$

# Example 06:

# This "git config" used to set up an alias for "external" command

$ git config --global alias.visual '!gitk'

# If you want to run an external command, rather than a Git subcommand. In that case, you start the command with a ! character.

$ git visual

# It demonstrates by aliasing git visual to run gitk:

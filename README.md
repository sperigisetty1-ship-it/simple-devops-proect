# simple-devops-proect
simple shell scripting 
ubuntu@ip-172-31-21-125:~/example.com$ git commit -m "This is my second version"
[master c441c76] This is my second version
 Committer: Ubuntu <ubuntu@ip-172-31-21-125.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 2 insertions(+), 1 deletion(-)
ubuntu@ip-172-31-21-125:~/example.com$ git log
commit c441c76b8cefc0ee9b62426a84e48e21f917d41e (HEAD -> master)
Author: Ubuntu <ubuntu@ip-172-31-21-125.ec2.internal>
Date:   Mon Sep 22 14:52:40 2025 +0000

    This is my second version

commit f45b4b7c4960772c88bc4e5f25a71844c4d6c53c
Author: Ubuntu <ubuntu@ip-172-31-21-125.ec2.internal>
Date:   Mon Sep 22 14:49:19 2025 +0000

    This is my first version
ubuntu@ip-172-31-21-125:~/example.com$ cat clculator.sh
cat: clculator.sh: No such file or directory
ubuntu@ip-172-31-21-125:~/example.com$ cat clculator
a=1
b=2
x=(a+b+c)
y=(a-b-c)
ubuntu@ip-172-31-21-125:~/example.com$ git log
commit c441c76b8cefc0ee9b62426a84e48e21f917d41e (HEAD -> master)
Author: Ubuntu <ubuntu@ip-172-31-21-125.ec2.internal>
Date:   Mon Sep 22 14:52:40 2025 +0000

    This is my second version

commit f45b4b7c4960772c88bc4e5f25a71844c4d6c53c
Author: Ubuntu <ubuntu@ip-172-31-21-125.ec2.internal>
Date:   Mon Sep 22 14:49:19 2025 +0000

    This is my first version
ubuntu@ip-172-31-21-125:~/example.com$ git reset --r hard f45b4b7c4960772c88bc4e5f25a71844c4d6c53c
error: ambiguous option: r (could be --no-no-refresh or --recurse-submodules)
usage: git reset [--mixed | --soft | --hard | --merge | --keep] [-q] [<commit>]
   or: git reset [-q] [<tree-ish>] [--] <pathspec>...
   or: git reset [-q] [--pathspec-from-file [--pathspec-file-nul]] [<tree-ish>]
   or: git reset --patch [<tree-ish>] [--] [<pathspec>...]

    -q, --[no-]quiet      be quiet, only report errors
    --no-refresh          skip refreshing the index after reset
    --refresh             opposite of --no-refresh
    --mixed               reset HEAD and index
    --soft                reset only HEAD
    --hard                reset HEAD, index and working tree
    --merge               reset HEAD, index and working tree
    --keep                reset HEAD but keep local changes
    --[no-]recurse-submodules[=<reset>]
                          control recursive updating of submodules
    -p, --[no-]patch      select hunks interactively
    -N, --[no-]intent-to-add
                          record only the fact that removed paths will be added later
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character

ubuntu@ip-172-31-21-125:~/example.com$ cat clculator
a=1
b=2
x=(a+b+c)
y=(a-b-c)
ubuntu@ip-172-31-21-125:~/example.com$

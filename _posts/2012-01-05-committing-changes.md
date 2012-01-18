---
layout: source
title: Committing Changes
source: http://book.git-scm.com/3_normal_workflow.html
---

Modify some files, then add their updated contents to the index:

    $ git add file1 file2 file3

You are now ready to commit. You can see what is about to be committed using git diff with the --cached option:

    $ git diff --cached

(Without --cached, git diff will show you any changes that you've made but not yet added to the index.) You can also get a brief summary of the situation with git status:

    $ git status
    # On branch master
    # Changes to be committed:
    #   (use "git reset HEAD <file>..." to unstage)
    #
    #   modified:   file1
    #   modified:   file2
    #   modified:   file3
    #

If you need to make any further adjustments, do so now, and then add any newly modified content to the index. Finally, commit your changes with:

    $ git commit

This will again prompt you for a message describing the change, and then record a new version of the project.

Alternatively, instead of running git add beforehand, you can use

    $ git commit -a

which will automatically notice any modified (but not new) files, add them to the index, and commit, all in one step.

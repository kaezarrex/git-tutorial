---
layout: source
title: Branching
source: http://book.git-scm.com/3_basic_branching_and_merging.html
---

A single git repository can maintain multiple branches of development. To create a new branch named "experimental", use

    $ git branch experimental

If you now run

    $ git branch

you'll get a list of all existing branches:

      experimental
    * master

The "experimental" branch is the one you just created, and the "master" branch is a default branch that was created for you automatically. The asterisk marks the branch you are currently on; type

    $ git checkout experimental

to switch to the experimental branch. Now edit a file, commit the change, and switch back to the master branch:

    (edit file)
    $ git commit -a
    $ git checkout master

Check that the change you made is no longer visible, since it was made on the experimental branch and you're back on the master branch.

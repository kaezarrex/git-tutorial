---
layout: source
title: Getting a Repository
source: http://book.git-scm.com/3_getting_a_git_repository.html
---

### Initializing a New Repo

    $ mkdir project
    $ cd project/
    $ git init
    Initialized empty Git repository in .git/

You've now initialized the working directory--you may notice a new directory created, named ".git".

### Cloning a Repo


In order to get a copy of a project, you will need to know the project's Git URL - the location of the repository. Git can operate over many different protocols, so it may begin with ssh://, http(s)://, git://, or just a username (in which case git will assume ssh). Some repositories may be accessed over more than one protocol. For example, the source code to Git itself can be cloned either over the git:// protocol:

    git clone git://github.com/transloc/TacoSalad.git

or over https:

    git clone https://github.com/transloc/TacoSalad.git

or over ssh:

    git clone git@github.com:transloc/TacoSalad.git

The git:// protocol is faster and more efficient, but sometimes it is necessary to use http when behind corporate firewalls or what have you. In either case you should then have a new directory named 'git' that contains all the Git source code and history - it is basically a complete copy of what was on the server.

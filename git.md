### Q. ***What is a repository in GIT?***


A repository contains a directory named .git, where git keeps all of its metadata for the repository. The content of the .git directory are private to git.


### Q. ***What is the difference between GIT and SVN?***

The difference between GIT and SVN is

a) Git is less preferred for handling extremely large files or frequently changing binary files while SVN can handle multiple projects stored in the same repository.

b) GIT does not support ‘commits’ across multiple branches or tags.  Subversion allows the creation of folders at any location in the repository layout.

c) Gits are unchangeable, while Subversion allows committers to treat a tag as a branch and to create multiple revisions under a tag root.


### Q. ***What is GIT stash?***

GIT stash takes the current state of the working directory and index and puts in on the stack for later and gives you back a clean working directory.  So in case if you are in the middle of something and need to jump over to the other job, and at the same time you don’t want to lose your current edits then you can use GIT stash.

### Q. ***What is the difference between ‘git remote’ and ‘git clone’?***

‘git remote add’  just creates an entry in your git config that specifies a name for a particular URL.  While, ‘git clone’ creates a new git repository by copying and existing one located at the URI.

### Q. ***How can you fix a broken commit?***


To fix any broken commit, you will use the command “git commit—amend”. By running this command, you can fix the broken commit message in the editor.


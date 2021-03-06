ParanoidAndroid
===============

Submitting Patches
------------------
We're open source, and patches are always welcome!
You can send patches by using these commands:

    cd <workspace>
    repo start <branch> AOSPA/<project>
    cd <project>
    git add -A
    git commit -a
    cd <workspace>
    repo upload AOSPA/<project>

Commit your patches in a single commit. Squash multiple commit using this command: git rebase -i HEAD~<# of commits>

If you are going to make extra additions, just repeat steps (Don't repo start again), but instead of git commit -a
use git commit --amend. Gerrit will recognize it as a new patchset.

To view the status of your and others patches, visit [ParanoidAndroid Code Review](http://gerrit.paranoidandroid.co)


Getting Started
---------------

To get started with ParanoidAndroid, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

To initialize your local repository using the ParanoidAndroid trees, use a command like this:

    repo init -u git://github.com/ModdedPA/manifest.git -b kitkat

Then to sync up:

    repo sync

For information on how to build, check [Here](https://github.com/AOSPA/manifest)

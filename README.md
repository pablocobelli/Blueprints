# Blueprints
Template managing and deploying via git.

Link: http://stackoverflow.com/questions/7106012/download-a-single-folder-or-directory-from-a-github-repo

Text: 

This is a pretty old question, but I figured this out today and I thought I'd leave this here for anyone else who has the same problem.

As all the previous answers have already noted, you are not allowed to download a single folder using Git. However, you ARE allowed to do this with subversion. This won't work on a regular git repo obviously, but if you're using GitHub you can actually check out using svn.

For example:

svn checkout https://github.com/foobar/Test/trunk/foo
trunk corresponds to master branch. You can use svn ls to see available tags and branches before downloading if you wish.

As of this writing, you can find the subversion URL for any repo on GitHub by clicking on "Subversion" at the bottom of the right sidebar.

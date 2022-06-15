## How to Use GitHub and BitBucket at the Same Time for One Project?

You can use multiple remote repositories with git. But you'll have to push separately into 2 of your remotes.

  > cd project

  > $ git remote add github https://github.com/your_user/your_repo.git 

  > $ git remote add bitbucket https://your_user@bitbucket.org/your_user/your_repo.git

<br />

Now in order to push changes to corresponding branch on github or bitbucket you can do this:

  > $ git push github master

  > $ git push bitbucket master

<br />

Same rule applies to pulling: you need to specify which remote you want to pull from:

> $ git pull github master

> $ git pull bitbucket master

<br />

If your project currently points to github, you can rename your current remote repository to github:

  > $ git remote rename origin github

<br/>

Finally, to see which remote will be fetched from:

  > $ git remote -v show

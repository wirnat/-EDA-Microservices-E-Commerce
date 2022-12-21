
## 1. Fork Enterprise POS to your repository and then clone.
```
$ git clone https://gitlab.com/<user>/enterprise-pos.git
```
If you have problem setup GIT for Gitlab on Linux, or error like "Permission Denied (publickey)", please setup your GIT for Gitlab.

## 2. Add Enterprise POS repository as additional git remote with name "upstream".
```
$ git remote add upstream https://gitlab.com/aksaratech/enterprise-pos.git
```
## 3. Get latest code from Enterprise POS.
```
$ git fetch upstream
```
This command you should run each time will contribute to ensuring you are working with the final code.

## 4. Create new branch base on Enterprise POS *develop* branch.
```
$ git checkout upstream/develop
$ git checkout -b 999-name-of-your-branch-goes-here
```

## 5. Write your code.
Do the best. Fix existing issues. Add features and more.
Make sure your code is working properly before uploading it :D.

## 6. Commit
add your files/changes that you want to commit to the staging area with
```
$ git add path/to/my/file.php
```
You can use the -p option to select the changes you want to commit.

Commit your changes with a clear description. You can add your issue number in #XXX format.
```
$ git commit -m "A brief description of this change which fixes #42 goes here"
```

## 7. Pool code last Enterprise POS to your branch.
```
$ git pull upstream develop
```
once again to make sure you are working with the latest code from Enterprise POS

## 8. Push your code to GitHub.
```
$ git push -u origin 999-name-of-your-branch-goes-here
```

## 9. Create a pull request.
Enter your repository on GitHub then click Pull Request. Choose a branch and add details in the comments. To link a "pull request" to an issue, add the issue number in the comments in the format #999.

> One "pull request" should only be for one change.

## 10. Someone will review your code.
Someone will review your code. Ask something, ask for changes and others. Do step 5 (you don't need to create a new "pull request"). If your code is accepted, it will merge and become part of Enterprise POS. If you are rejected, don't be discouraged, everyone has their own considerations :D.

## 11. Clean up.
If it is finished, either because it is accepted or rejected. Clean your local repository.

```
$ git checkout master
$ git branch -D 999-name-of-your-branch-goes-here
$ git push origin --delete 999-name-of-your-branch-goes-here
```
## 12. Thanks.
If there is something wrong in this post, please forgive me. I'm still a newbie bro :D
Regards.

Summary
```
$ git clone https://github.com/<user>/enterprise-pos.git
$ cd enterprise-pos
$ git remote add upstream git://github.com/sangkil/enterprise-pos.git

$ git fetch upstream
$ git checkout upstream/master
$ git checkout -b 999-name-of-your-branch-goes-here

/* do your magic, update changelog if needed */

$ git add path/to/my/file.php
$ git commit -m "A brief description of this change which fixes #42 goes here"
$ git pull upstream develop
$ git push -u origin 999-name-of-your-branch-goes-here
```

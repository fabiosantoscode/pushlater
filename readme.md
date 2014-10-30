# What?

Use this to work offline with git.

When you have no internet connection, you can't `git push`. That's why I created `pushlater`. Call `pushlater` with the same arguments as `git push`. When you have internet, call `pushlater --now` and your repos will be pushed. In case the git push fails for some reason, you will be notified.


# Demo

```
$ git remote add origin git@github.com:fabiosantoscode/pushlater.git
$ pushlater --set-upstream origin master
A push shall occur later. Just run "pushlater --now" when you have internets!
$ pushlater --now
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 943 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To git@github.com:fabiosantoscode/pushlater.git
 * [new branch]      master -> master
 Branch master set up to track remote branch master from origin.
$ 
```

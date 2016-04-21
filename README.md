# special-characters
A repository full of files that desktop versions of Git will hate, all made in the Web UI, which evidently has no form of input validation. This is an example repository for an issue I am soon to make

Not all of the characters I have demonstrated are bad, such as the brackets, but some, such as the asterisk `*` undoubtedly are. 

Cloning this repository will create untold confusion: here is a `git pull` then `git status` of my repository, straight after I added the first dodgy file, in this case with a colon: 

```
C:\Users\User\Documents\Benji\Coding\special-characters>git pull
Enter passphrase for key '/c/Users/User/.ssh/id_rsa':
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From github.com:benjimarshall/special-characters
   60a8c0e..e446f0a  master     -> origin/master
Updating 60a8c0e..e446f0a
Fast-forward
 colon:file.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 colon:file.txt

C:\Users\User\Documents\Benji\Coding\special-characters>git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        colon

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\User\Documents\Benji\Coding\special-characters>
```

Incidentally, I accidently made the folder `asteriskfile`, and I can't delete the folder in the Web UI, nor can I sort it out on a Git repo on my computer unless I let it clean up all of my special character names by deleting the files (which potentially could have useful data in).

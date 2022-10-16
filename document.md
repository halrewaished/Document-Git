## 3-way merge :

When there is not a linear path to the target branch, Git has no choice but to combine them via a 3-way merge.
3-way merge use a dedicated commit to tie together the two histories.


## Commands to get 3-way merge:

1- create a new branch named ( First ). 
[ git branch first ].



2- switch to the new branch ( First ). 
[ git checkout first ].

3- create new commits. 
[ git commit -m “ start commit” ].

4- switch again to the ( main ) branch. 
[ git checkout main ].

5- create new commits. 
[ git commit -m “ new commit” ].

6- create merge. 
[ git merge first ].

Here will present merge conflict. 
To handle the conflict it must edit the content of the affected files with visual indicators that mark both sides of the conflicted content. These visual markers are: <<<<<<<, =======, and >>>>>>>.

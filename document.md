## 3-way merge :

When there is not a linear path to the target branch, Git has no choice but to combine them via a 3-way merge.
3-way merge use a dedicated commit to tie together the two histories.


## Commands to get 3-way merge:

1- create a new branch named ( First ). 
[ git branch first ].

<img width="416" alt="Screenshot 1444-03-20 at 1 43 36 PM" src="https://user-images.githubusercontent.com/103143504/196101438-b5298b50-703e-4427-a3ed-3d8486287b45.png">

2- switch to the new branch ( First ). 
[ git checkout first ].

3- create new commits. 
[ git commit -m “ start commit” ].

<img width="617" alt="Screenshot 1444-03-20 at 1 43 51 PM" src="https://user-images.githubusercontent.com/103143504/196101522-b27ae919-9403-4198-bd64-00188fab131f.png">


4- switch again to the ( main ) branch. 
[ git checkout main ].

5- create new commits. 
[ git commit -m “ new commit” ].

<img width="617" alt="Screenshot 1444-03-20 at 1 44 01 PM" src="https://user-images.githubusercontent.com/103143504/196101615-793be88c-c37f-432c-b26a-4614c7c386bf.png">


6- create merge. 
[ git merge first ].

<img width="669" alt="Screenshot 1444-03-20 at 1 44 12 PM" src="https://user-images.githubusercontent.com/103143504/196101643-0786663e-20c5-45cc-af79-69b645f1212c.png">


Here will present merge conflict. 
To handle the conflict it must edit the content of the affected files with visual indicators that mark both sides of the conflicted content. These visual markers are: <<<<<<<, =======, and >>>>>>>.

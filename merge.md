Fast forward merge can be performed when there is a direct linear path 
from the source branch to the target branch. In fast-forward merge, git 
moves the source branch pointer to the target branch pointer without 
creating an extra merge commit.    



a main branch with 3 commits.


<img width="442" alt="Screen Shot 1444-03-20 at 1 07 50 PM" src="https://user-images.githubusercontent.com/103157455/196116322-b93e04d7-f66a-4e85-8514-374f0c28ad19.png">







create a branch called  New_Branch.  both New_Branch and main are pointing 
to the same commit  



    $ git branch New_Branch
	
<img width="604" alt="Screen Shot 1444-03-20 at 2 06 48 PM" src="https://user-images.githubusercontent.com/103157455/196116631-28be4559-2017-4a23-b4cd-17c3625542d2.png">
	










 switch to the New_Branch branch and do a couple of commits. Now we need 
to bring the changes to the main branch. There is a linear path from 
feature to main.   


    $git checkout New_Branch
	



<img width="659" alt="New Branch" src="https://user-images.githubusercontent.com/103157455/196116994-28295d9f-91f9-4bee-a94f-653c5319f80c.png">







In order to merge the changes to the main branch, all git has to do is to 
change the pointer of main forward. This is what we call fast-forward 
merge.



<img width="648" alt="forward" src="https://user-images.githubusercontent.com/103157455/196117617-e21be25d-e398-40df-906b-8d2e1cb07241.png">








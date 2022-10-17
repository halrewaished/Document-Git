Fast forward merge can be performed when there is a direct linear path 
from the source branch to the target branch. In fast-forward merge, git 
moves the source branch pointer to the target branch pointer without 
creating an extra merge commit.    



a main branch with 3 commits.









create a branch called  New_Branch.  both New_Branch and main are pointing 
to the same commit  



    $ git branch New_Branch
	
	










 switch to the New_Branch branch and do a couple of commits. Now we need 
to bring the changes to the main branch. There is a linear path from 
feature to main.   


    $git checkout New_Branch
	







switch to the feature branch and do a couple of commits, then bring the 
changes to the main branch. There is a linear path from feature to main.




In order to merge the changes to the main branch, all git has to do is to 
change the pointer of main forward. This is what we call fast-forward 
merge.




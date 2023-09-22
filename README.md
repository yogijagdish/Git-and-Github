<h1 align="center"> Git and Github </h1>

<dl>
  
  <h2 align="center"> Configuaration </h2>
  <dt> git config --list </dt>
  <dd> to see configuaration of the git </dd>
  <dt> git config --global user.email "example@gmail.com" </dt>
  <dd> to set or change the email of the user in git </dd>
  <dt> git config --global user.name "username" </dt>
  <dd> to set or change the username in the git </dd>
  
  <h2 align="center"> Status </h2>
  <dt> git status </dt>
  <dd> shows the status of the action conducted on the git </dd>
  <dt> git diff --staged </dt>
  <dd> shows the difference between two version of the staged files </dd>
  
  <h2 align="center"> To Add File To Staging Area </h2>
<dt> git add filename </dt>
<dd> to add single file of particular filename in staging area </dd>
<dt> git add filename1 filename2 </dt>
<dd> to add multiple files to staging area of particular name in git </dd>
<dt> git add . </dt>
 <dd> to add all files in git </dd>
  
<h2 align="center"> To commit changes in git </h2>
<dt> git commit -m "message" </dt>
<dd> to add file to local repository with a unique and distinctive message </dd>
 <dt> git commit -am "message" </dt>
 <dd> adds file to staging area and then to local repository </dd>
  
  <h2 align="center"> To View Commit History </h2>
  <dt> git log </dt>
  <dd> shows the detail history of commit </dd>
  <dt> git log --oneline </dt>
  <dd> shows the detail history of commit command in oneline </dd>
  
  <h2 align="center"> To Go To Previous Version Or Branch </h2>
  <dt> git checkout #number </dt>
  <dd> takes us to the version of the given hash number </dd>
  <dt> git checkout branchname </dt>
  <dd> takes us to the required branch </dd>
  
  <h2 align="center"> Add and remove remote origin </h2>
  <dt> git remote add origin "url of the github" </dt>
  <dd> adds the orgin or path of the github repo </dd>
  <dt> git remote remove origin </dt>
  <dd> removes the origin path of the github </dd>
  <dt> git remote -v </dt>
  <dt> git remote show origin </dt>
  <dd> shows us the origin path of the github </dd>
  
  <h2 align="center"> Push The Files To The Github </h2>
  <dt> git push origin main/master </dt>
  <dd> pushes all the changes to the main branch in github </dd>
  <dt> git push origin branch_name </dt>
  <dd> pushes all the change in the code to the specified branch </dd>
  
  <h2 align="center"> Cloning The Project From Github </h2>
  <dt> git clone "url of the github account" </dt>
  <dd> clones the whole project in our computer </dd>
  
  <h2 align="center"> Branching In Git </h2>
  <dt> git branch branch_name </dt>
  <dd> creates new branch in the git </dd>
  <dt> git branch </dt>
  <dd> shows all the branch created in the git </dd>
  
  <h2 align="center"> Merging Files Of The Branch </h2>
  <dt> git merge "branch_name" </dt>
  <dd> note to make sure to go to the main branch where we want to merge the files </dd>
  <dt> git merge --no-ff "branch_name" </dt>
  <dd> merges the file with no fastforward </dd>
  <dt> git branch --merged </dt>
  <dd> shows merged branch </dd>
  <dt> git branch --no-merged </dt>
  <dd> shows not merged branch </dd>
  
  <h2 align="center"> Reset Our Head To Previous Version </h2>
  <dt> git reset --head #number_of_previous_version </dt>
  <dd> used when we want to discard all the changes and restart from the previous version </dd>
  
  <h2 align="center"> Deleting Branch In Git </h2>
  <dt> git branch -d "branch_name" </dt>
  <dd> deletes the branch but rejects if it is not merged </dd>
  <dt> git branch -D "branchname" </dt>
  <dd> deletes the branch even if it is not merged </dd>
  
  <h2 align="center"> Pulling The Files From The Github Repository </h2>
  <dt> git pull origin main/master/branch_name </dt>
  <dd> pulls the chnages done by other to our code </dd>
  
  <h2 align="center"> Tagging In Git </h2>
  <dt> git tag -a tag_name -m "message" </dt>
  <dd> adds tags in the git which is used to check milestones while coding </dd>

  <h2 align="center"> Stashing In Git </h2>
  <dt> git stash </dt>
  <dd> puts all your current changes in hold and allows you ro pull new data form other branch without pushing your code </dd>
  <dt> git stash pop </dt>
  <dd> pops all your stashed files after you pull the branch </dd>

   <h2 align="center">   Fetching In Git </h2>
  <dt> git fetch --all </dt>
  <dd> fetch all the branch from git hub similar to git pull </dd>
 
  </dl>

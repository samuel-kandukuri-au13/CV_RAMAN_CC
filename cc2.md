
Let us assuse that blue is master branch
		   purple is A branch
		   green is B branch

First commit:

Create a new file reposiory and initiate git and then create a new Readme.md file
		
		$touch readme.md
		$git add .
		$git commit -m " A new file has been created in the master branch"
		$git branch A
		$git branch B
Second commit:

	make some changes in the Readme file and commit
		$ echo this is first line from master branch>>readme.md
		$git add .
		$ git commit -m "second commit made from master"

Third commit(purple)

	We have to switch to A branch and  make changes to the file and commit.

		$ git checkout A
		$ echo this is first line from branch A>>readme.md
		$ git add .
		$ git commit -m "first commit made from A"

fourth commit(purple)
	make some changes in the Readme file and commit
		$ echo this is second line from branch A>>readme.md
		$ git add .
		$ git commit -m second commit made from A"

fifth commit (blue)
	switch to master branch make some changes in the text file and commit
		$ git checkout master
		$ echo this is second line from master>>readme.md
		$ git add .
		$ git commit -m "third commit made from master"

sixth commit (blue)
	make some more changes to the readme file and commit
		$ echo this is third line from master>>readme.md
		$ git add .
		$ git commit -m fourth commit made from master"
		
seventh commit(green)
	switch to B branch and make changes to the readme file
		
		$ git checkout B
		Switched to branch 'B'
		$ echo this is first line from B>>readme.md
		$ git add .
		$ git commit -m "first commit from B"

eighth commit(green)
	Make some changes to the readme file and commit
		$ echo this is second line from B>>readme.md
		$ git add .
		$ git commit -m "second commit from B"

ninth commit(blue)
	make some cheanges to the readme file and commit changes from master branch
		$ git checkout master
		$ echo this is the last line from master>>readme.md
		$ git add .
		$ git commit -m "this is the last commit from master"

	MERGE BRANCH B into master--------got error
		$ git merge B
	MERGE BRANCH A into master
		$ git merge A
		

							link https://github.com/samuel-kandukuri-au13/merge
		


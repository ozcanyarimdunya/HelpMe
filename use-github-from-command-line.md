## How to use github from command line

    git config --global user.name="username"
    git config --global user.email="useremail"

 
That's the all for configurations

##### For example you want commit one.py file in the /home/user/MyFile/1.py

#####Open a Terminal and go inside /home/user/

    git init    	    # create a git initializer
    git add MyFile 	    # add the file you want to commit to repo
    git commit -m "First initialize"
    git remote add origin https://github.com/username/RepoFile/repo.git
    git remote -v
    git push origin master 


#####Then everytime you add,remove a file or make change first

    git status 		    # check the status
    git add filename	# add the file or the changes in the file to repo
    git commit -m "file added"
    git push origin master
    git rm filename	    # remove the file from the repo
    git commit -m "file removed"
    git push origin master 

#####For the change on github.com 
    git pull            # merge the changes
##### That's it !

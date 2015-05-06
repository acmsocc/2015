# SoCC 2015 Website

## Instructions for making changes to website

### Step 1: Github account

If you don't have a github account, please create one at https://github.com

### Step 2: Access to repository

If you are new to github or already have an account, you need permission to work in the repository. Ask your administrator 
to provide permissions.

### Step 3: Install Git in your laptop/computer

If you don't have git installed in your computer, please follow the instructions here. 

### Step 4: Checkout repository

From your unix terminal window use the following command to check out the repository

> git clone https://github.com/acmsocc/2015.git

A directory called 2015 will be created which houses the repository. The repository might not contain any code since it is the master. You need to check out the branch called gh-pages. 
For checking out the branch, use the following

> git checkout gh-pages

### Step 5: Edit the repository

You can edit the pages or add new pages as you like

### Step 6: Committing to the repository

In order to know the list of newly added files or the modified files do 

> git status 

Now do git add for the untracked files by using the following command

> git add <filename>

You should use git commit to push the changes. Note it will commit to the local repository only

> git commit -m "Your Message"

### Step 7: Push the repository 

You can push the changes to main branch by doing the following

> git push 

After these only the pages will show up in the website

### Step 8: For previewing the site

If you would like to preview the site before committing, you need to install Jekyll. You can follow the instructions at http://jekyllrb.com/  

> gem install jekyll

Once you have installed Jekyll, cd to your repository directory and in a separate window do the following

> jekyll build --watch

This will not terminate. In another terminal window, you can edit or change the files in the repository. 

In order to preview the site, open up a browser and in it open the url 

file://\<absolute-path-of-directory-where-the-repo-is>/_site/index.html

All you have to is keep refreshing to get the new site previewed before you do the commit.

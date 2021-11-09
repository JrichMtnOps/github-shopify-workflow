GIT FLOW PROCESS for integrating with Shopify
Say goodbye to THEME KIT!!


Initialize git by running [git init]

Start new repo in github and follow steps there 
(skip setting up main branch we will do something later)

Go to Shopify themes and under theme library click add theme dropdown and select [ connect from git hub ]
    - Select what Repositories you want this store to access
    - install
    - (may need to run through incognito window due to   caching)

We can now set this to our live theme only after double checking that everything is working properly!

Lets set up our Dev Branch 
run [git checkout -b <branchname>]
if we want to rename after because just use [git branch -m <oldname><newname>]
to switch between branches we can just use [git checkout <branchname>]

Now that we have our new branch we can add it to our theme library in shopify using the same method we did above for the master theme

to make sure there are no conflicts we will want to run git merge master while in our staging branch and adjust any merge conflicts (if there are merge conflicts we want them to happen on the staging branch NOT the master branch)

after working on merge conflicts (if any) we now need to go to our master branch with [git checkout master] and then merge with our staging branch with [git merge staging]


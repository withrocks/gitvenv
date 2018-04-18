# What 

Creates virtual environments for all (or some) branches in a github repo.

# Why 

You have a (potentially shared) dev server that is hosting the code on your dev branch, but you want developers to be able to test a feature branch automatically by just switching virtual environments (here I'm using conda):

* Push a change to the branch `dev1/0/feature1`
* A server running this tool as a daemon pulls down these changes automatically and synchs with the venvs
* A dev can now run `source activate dev1_0_feature1` to test the branch
 

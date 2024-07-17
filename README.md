#### Instructions for uploading project code to github

Returnable code for UK Biobank approved project 15147 is made publicly available at [https://github.com/ukb15147](https://github.com/ukb15147)

Suggested approach to establish a code repository for a new publication:

 * If using git for the first time or from a new machine, set global user.name and user.email options:

        git config --global user.name "USERNAME"
        git config --global user.email "NAME@DOMAIN.com"

 * Collect together code/scripts to be made available in one directory. Don't include anything else in this directory
 * Create a **README.md** file describing the code (e.g. using Obsidian on mac)
 * Create a .**gitignore** file to exclude hidden files. Contents as follows:

        # Ignore all files beginning with .
        .*
        #. But keep .gitignore
        !.gitignore

 * Initialise and initially commit the git repository:

        git init
        git add --all
        git status
        git commit -m "Initial commit"
        git status

 * On github, create a new repository under the **ukb15147** "organisation", giving it a short, suitably descriptive name. Once set up, the front page of this repository will provide a repository URL.
 * In the local directory, push the code to the github repository.

        git branch -M main
        git remote add origin https://github.com/ukb15147/REPOSITORYNAME.git
        git push -u origin main

 * Check the code is now viewable on github

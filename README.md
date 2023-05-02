# branch-example
Example files to help learn branching

## About
This excercise is meant to be done with two or more people. The idea is to allow practicing creating and merging branches with simple text files. Markdown files are used but really any simple text file (ie .txt) could be used as well.

It's created for people who already have some knowledge of Git and GitHub. The commands shown here are ones to be entered into the terminal. There are also tools that can be used to perform these ations in a more visual way.

## Setup
Before you start, everyone in the group will need GitHub accounts.

1. **Create Repo from Template**: One person in the group creates a repository baed on this one (click the Use this Template button).
2. **Add Collaborators**: everyone else in the group gives their Github usernames to the peron who created the repository. That person then can [add them a collaborators](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository) to the repository.


## Branching and Merging with Individual Files
4. **Add name to People folder**: everyone should go in and create a branch. Name the branch with your name. For example if your name is jane
    - `git checkout -b jane`
    - _note: two branches can't share the same name so if two people share the same name, use last name, nickname etc._
5. **Create Personal File**: in the new branch each person should create a file for themselves in the __people__ folder. 
    - remember to commit the file after creating. For example: 
    - `git add jane.md`
    - `git commit -m "added file for jane"`
7. **Switch back to the main branch:** after creating and committing the new file, switch to __main__. we do this because when you merge you merge another branch into the branch you're currently in. Since we want each person to merge their branch into the main branch, people should move to main before merging. 
    - `git checkout main`
    - note that we dont' add `-b` because that is only added when creating a new branch.
    - if you're using a visual tool, you may be able to merge without switching branches.
9. **Merge person branch into Main:**  merge it into the __main__ branch. To merge the _jane_ branch we made earlier we would enter:
    - `git merge jane`

If everyone did this with unique file names then all files from all people should be now merged back into the main branch and the people folder should have a file for each person.


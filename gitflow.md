Our gitflow is divided into four (4) major parts

1. Fetching the latest master
2. Creating/using existing branch to work.
3. Commiting changes
4. Pushing to remote branch and raising PRs


- **Fetching the latest master**
    - **first time**: `git clone #repo_link` (preferably use ssh) and follow the instrustion in the `Readme.md` file.

    - **subsequently**: Navigate to `master` branch using `git checkout master` then `git pull` or `git pull origin master`.

    - **NB: NEVER tamper with the master branch, ALWAYS let the status be clean to avoid remote merge conflicts**.

- **Creating/using existing branch to work**
    - **new branch**: Create  new branch using `git checkout -b #branch_name`

    - **existing branch**: Navigate to branch using `git checkout #branch_name`, then `git rebase master`

- **Commiting changes**
    - **first time**: `git add .` then `git commit -m '#commit_message'`.

    - **subsequently**:`git commit -am '#commit_message'`.

- **Pushing to remote branch and raising PRs**
    - If you are not on the working branch, navigate there

    - `git push` or `git push -u origin #branch_name`

    - If you had to do a `git rebase master` from step 2 in the gitflow, then do `git push --force` or `git push -u origin #branch_name --force`

    - **NB: Before pushing to the remote branch and raising a PR, ALWAYS deploy your code to staging and test, EXCEPT you want to tag the PR as draft or WIP**.

        - **Deploying to staging**
            - `git checkout staging`

            - `git pull` or `git pull origin staging`

            - `git merge #branch_name`

            - `git push` or `git push -u origin staging`




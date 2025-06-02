# git

> What is git ?
Git is a version control system used by almost all the organizations to version control their development and parallel development using branches.  
Once you're good with the changes that you made, we will publish the code to GITHUB / GITLAB / BIT-BUCKET

> What is GitHub, GitLab, BitBucket ?
These are centralised version control system

> What is a branch in GIT ?

```
    A branch is a copy of the code which allows the developers to test without touching the main code and this helps multiple developers to contribute parallely.

    By default, main is the branch which should be the source of truth or production ready code.

```

> When ever we want to do some changes to the production environment, it has to go through a process called as Change Management Process.
And the associated board is called as CAB or Change Advisory Board.

    *   Changes to the production would only be done during off business hours or out of business hours.

> Why it's important to follow the change management process while relesing the changes to production ?


> How do we control the parallel development of the apps ?

```
   A branch is a version of your repository, or in other words, an independent line of development. 
   
   A repository can contain multiple branches, which means there are multiple versions of the repository.

   Among all, main / master branch is something which you should always a checkout to create a new /feature branch
```

> Git Branch Naming Strategy

Branch naming strategy will be based on the org choice and here are the industry standards:

    Typically, you either work on:
        1)feature/expense-app-2   [ This is to identify the branch that you're working has a new feature ]
        2)hotFix                  [ hotfix/xyz-123 ]
        3)bug                     [ bug/payments-correction ]

You release a feature to production and that has package-xyz and that package-xyz is causing issue and the fix is package1-abc needs to be added. 

In this cases, we are going to do the change fix on the pre-prod first and then immediately to production

        Dev --->  QA ---> Pre-Prod ----> CAB Request ----> Prod

> A hotfix in software development is a quick and targeted update to fix a critical bug or issue in a production environment. It’s usually applied outside the normal release cycle because the issue is urgent and negatively affects users, business operations, or security.


> Git Commands

```
    $ git branch                    // Shows you which branch you're in.
    $ git branch brachName          // This creates a branch with name branchName from the branch you're in.
    $ git checkout branchName       // This is to switch to the branch named branchName.
    $ git checkout -b branchName    // This creates a branch branchName and switches your current branch to branchName.
    $ git push origin branchName    // This push to the branchName mentioned.
    $ put pull origin branchName    // To pull changes from the specific branch
```
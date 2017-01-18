> [Git user guide](https://git-scm.com/documentation)
>
> [Git tutorial](https://www.atlassian.com/git/tutorials/)
>
> [Git cheat sheet](https://www.git-tower.com/blog/git-cheat-sheet/)

## Examples:

|Upstream        |Origin                    |Local                   |
|---------------:|-------------------------:|-----------------------:|
|Team repo       |My remote repo            |Local repo              |
|develop         |develop / featureBranch   |develop / featureBranch |

- set up a new local git repo

    ```$git init```

- set the upstream _(team repo)_

    ```$git remote add upstream <team-repo-github-url>```

- pull the develop branch from upstream _(synchronize with team repo)_

    ```$git pull upstream develop```

- create a new local feature branch

    ```$git checkout -b <featureBranch>```

    or

    ```$git branch <featureBranch>```

- switch to another branch

    ```$git checkout otherBranchName```

- commit changes to the local branch

    ```$git commit -s -m "<type necessary comments>"```

- push local feature branch to remote and create a remote feature branch

    ```$git push origin <featureBranch>```

- push the local feature branch to the remote dev branch

    ```$git push origin <featureBranch>:develop```

- Untrack files

    ```$git update-index --assume-unchanged <path/to/file>```

    or

    ```$git rm -r --cached <path/to/file>```

- Start keeping track

    ```$git update-index --no-assume-unchanged <path/to/file>```

- Change the remote url

    ```$git remote set-url <upstream or origin> <corresponding-github-url>```


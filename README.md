# GitHub CLI

## Prerequisites:
- Install [Git SCM](https://git-scm.com/downloads)
- Install [GitHub CLI](https://cli.github.com/)

## Loose Agenda:
- Gain familiarity with GitHub CLI and related workflows

## GitHub CLI Step by Step


### Create a repository

In a terminal, enter the following command
```
gh repo create github-cli
```

### Clone a repository

In a terminal, change directory to where you wish to put the newly created git repository then enter the following command

```
git clone PUT-LINK-HERE
```

Note - you can find the link by opening the newly created repository in your internet browser and clicking the green Code button near the top of the page. There is a clipboard icon which will copy the link for you.

### Commit to Main

Add a text file into the cloned repository and run the following commands

```
git add .
git commit -m "Initial Commit"
git push origin main
```

### Commit to Branch

Add another text file into the cloned repository and run the following commands

```
git checkout -B nonzerodays-branch
git add .
git commit -m "Initial Commit"
git push origin nonzerodays-branch
```

### Create a Pull Request

```
gh pr create --title "Added text file" --body "It's a non-zero text file"
```

### Merge a Pull Request

In a command prompt enter the following command
```
gh pr merge nonzerodays-branch --squash
```

Typically, I delete the branch after completing a pull request. 


Congratulations on a non-zero day!

# 💡 Summary
- [What is Git](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#what-is-abstract-data-types)
- [You must know](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#what-is-abstract-data-types)
- [Most Used Comands](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#what-is-abstract-data-types)
- [Branch View](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#what-is-abstract-data-types)
- [Git Cheat Sheet](https://github.com/LuisValgoi/5Things1DevShouldKnow/blob/master/DataStructures/DATA_STRUCTURES.md#what-is-abstract-data-types)
---
---
---
# What is Git?
* Git is a distributed version control system and source code management system.

## Who uses it?
* All people who are involved in a software development team/process.

## Advantages
* Distributed model
    * This means your work is your own. You can let others see only what is necessary.
    * Not everything has to be public. 
    * Very fast.
* Branching and merging are easy
    * It feels like a natural part of the workflow. 
    * They are cheap so you can branch whenever you want.
* Data integrity is assured
    * Because git uses SHA1 trees, data corruption due to external reasons can be easily detected.

## Disadvantages
* Steep learning curve: Many commands with many options.
* Commands are non-intuitive.
* Binary files are a big no (If your project has non-text files that are updated frequently).


# You must know:

**Repository:** It is a local storage of software packages which can be recovered and installed on a computer.

**Remote** When your artefacts are directly on the Git Server.

**Branch** It is the term we use for a variaton from the production/master/final(trunk) code.

**Master** It is the term we use for where your final/production/stable code must be.

**Fork** It is the term we use when we want to take the source code from a program and to develop a entirely new program.

**Checkout** When we want to download the repository with its current status.

**Clone** When we want to fetch the repository from the remote git server.

**Log** Is the term we use to extract the history of commits of the current prject.

**Add/Stage** When we use for stage files into the staging process of the Git before the commit.

**Commit** When we add the latest changes to the source code to the repository.

**Push** When we want to transfer the last commit(s) to a remote server.
 
**Fetch** When we update our local code according to the code on the remoter server.

**Pull** When we update our local code according to the code on the remoter server followed by the merge of these both code.

**Pull Request** Is a method of submitting contributions to an open development project.

**Merge** When we want to combine two pieces of code into one.

**Diff**: When we want to see the differences between two codes right before merging it.

**Deploy**: Is the term we use when we want to release our application to its production phase.


---
---
---

# Most Used Comands

## Check Git Proxy
`git config --global http.proxy`

## Set Git Proxy for SAP-Corporate
`git config --global http.proxy "http://proxy:8080"`

## Unset Proxy for SAP-Internet
`git config --global --unset http.proxy`

## Create Local Branch
`git checkout -b <branch>`

## Add Changes
`git add <fileName or *>`

## Commit Changes
`git commit -am "msg"`

## Push to Local Branch
`git push`

## Push to Remote Branch
`git push -u origin {the_remote_branch}`

## Delete Local Branch
`git branch -d {the_remote_branch}`

## Delete Remote Branch
`git push origin --delete {the_remote_branch}`

## Add Remote Upstream
`git remote add upstream <UrlMainRepoLinkSSH>`

## Fetch Upstream
`git fetch upstream`

## Update Forked from <master-main-repo>
`git pull upstream master`

## Set Local Upstream Branch
`git branch --set-upstream my_branch origin/my_branch`

---
---
---

# Branch View
![alt text](https://cdn-images-1.medium.com/max/1600/1*0obEIkTsoaponIib6i9Xog.png)

# Git Cheat Sheet 
![alt text](https://preview.ibb.co/eq81sn/download.png)
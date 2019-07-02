# 💡 Summary
- [Continuos Integration]()
- [Continuous Delivery]()
- [Continuous Deployment]()
- [Overview of CD/CI]()
- [How to do it]()
---
---
---
# Continuos Integration
* It is a strategy for how a developer can integrate code to the mainline continuously.
* "Developers practicing continuous integration merge their changes back to the main branch as often as possible."
* The developer's changes are validated by creating a build and running automated tests against the build.
* Continuous integration puts a great emphasis on testing automation to check that the application is not broken whenever new commits are integrated into the main branch.

# Continuous Delivery
* It is an extension of continuous integration to make sure that you can release new changes to your customers quickly in a sustainable way.
* It is the ability to get changes of all types—(new features, configuration changes, bug fixes) into the hands of users, safely and quickly in a sustainable way.
* We achieve all this by ensuring our code is always in a deployable state.
* If you truly want to get the benefits of continuous delivery, you should deploy to production as early as possible to make sure that you release small batches.

# Continuous Deployment
* Continuous deployment goes one step further than continuous delivery.
* Every change that passes all stages of your production pipeline is released to your customers.
* There isn't a Release Day anymore

# Overview of CD/CI.
![alt text](https://i.imgur.com/upb7y4s.png)

# How to do it?

| Practice              | What you need (COST)                                                   | Benefits (GAIN)                                                    |
|-----------------------|------------------------------------------------------------------------|--------------------------------------------------------------------|
| Continuos Integration | Automated Tests (each new feature)                                     | Less bugs into prod                                                |
| Continuos Integration | A Continuous Integration Server (run tests each new commit)            | Developers are alerted as soon as they break the build             |
| Continuos Integration | Devs need to merge changes as often as possible                        | Testing costs are reduced drastically                              |
|						|																		 |																	  |
| Continuos Delivery    | strong foundation in continuous integration                            | Complexity of deploying software has been taken away               |
| Continuos Delivery    | Deployments need to be automated. The trigger is still manual          | You can release more often (less pressure on decisions)            |
|						|																		 |																	  |
| Continuous Deployment | Testing culture needs to be at its best                                | No need to pause development for releases                          |
| Continuous Deployment | Quality of your test suite will determine the quality of your releases | Deployments pipelines are triggered automatically for every change |
| Continuous Deployment | Documentation process will need to keep up                             | Releases are less risky and easier to fix                          |

# To Remember
> "One of the traditional cost associated with continuous integration is the installation and maintenance of a CI server. But you can reduce significantly the cost of adopting these practices by using a cloud service like Bitbucket Pipelines."

> "By simply adding a configuration file at the root of your repository you will be able to create a continuous deployment pipeline that gets executed for every new change pushed to the main branch."
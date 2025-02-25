# Arlo's Commit Notation

## Upper case: Deliberate behavior changes

| Prefix  | Meaning                                                   |
| ------- | --------------------------------------------------------- |
| F       | Feature                                                   |
| B       | Bug                                                       |

## Lower case: Low risk

| Prefix  | Meaning                                                   |
| ------- | --------------------------------------------------------- |
| c       | comments (add/delete)                                     |
| d       | developer documentation changes (not end-user facing)     |
| e       | environment (non-code) changes                            |
| t       | Test only                                                 |
| r       | Provable Refactoring                                      |
| a       | Automated formatting                                      |

## Three characters: The danger zone!

| Prefix  | Meaning                                                   |
| ------- | --------------------------------------------------------- |
| !!!     | non-provable refactoring                                  |
| ***     | does not compile intermediate step                        |

# Description

[Arlo's](https://twitter.com/arlobelshee) Commit Notation is a way of making small commits that show the risk involved in each step. It is particulary useful in legacy systems. 

# Provable Refactorings

If you can get a series of commits that is all lowercase commits, you can deploy without the need for Regression Testing, or lengthy conversations about accepting the pull request to trunk.

A provable refactoring requires the burden of proof. The main methods of proof are
* automated refactoring via tool
* Scripted manual refactoring, using the compiler to verify each step
* Very Highly tested code, with the tests providing proof

# Living Documentation

We invite you to submit pull requests to help evolve this notation and methodology.

# Bookworm Reads Contribution Guide

We'd love for you to contribute to our source code and to make Bookworm Reads technology even better than it is today! Below are the guidelines we'd like you to follow.

For Issues, Pull Requests, and code, please refer to our [Inclusive Language Guide][lang].

## Questions, Bugs, Features

### Questions and Problems

We want to keep GitHub Issues dedicated to bug reports and feature requests. Any general support questions are better directed towards a dedicated support platform, the best being the [Bookworm Reads Discord][discord], the second best being our [support email][support-email].

### Issues and Bugs

If you find a bug in the source code or documentation, you can help by submitting an Issue to the respective GitHub repository. Even better, you can submit a Pull Request with a fix.

### Feature Request

You can request a new feature by submitting an Issue to the respective GitHub repository.

### Improving Documentation

Should you have a suggestion for the documentation, you can open an Issue and outline the problem or improvement you have - however, creating the documentation fix yourself is much better!

## Issue Submission Guidelines

If you want to help improve our code, even something as small as just a fix in the docs, it's a good idea to let others know what you're working on to minimize duplication of effort. Create a new Issue (or comment on a related existing one) to let others know what you're working on.

Before you submit your Issue search the archive, maybe your question was already answered or problem resolved.

If your Issue appears to be a bug, and hasn't been reported, open a new Issue. Help us to maximize the effort we can spend fixing Issues and adding new features, by not reporting duplicate Issues.

The "new issue" form contains a number of prompts that you should fill out to make it easier to understand and categorize the Issue.

**If you get help, help others. Good karma rulez!**

## Contribution Requirements

Before you can build one of our libraries, you must install and configure the following dependencies on your machine:

* [Git][git]: The [Github Guide to Installing Git][git-setup] is a good source of information.

* [Node.js (LTS)][node]: We use Node to generate the documentation, run a development web server, run tests, and generate distributable files. Depending on your system you can install Node either from source or as a pre-packaged bundle. We recommend using [nvm][nvm] (or [nvm-windows][nvm-windows]) to manage and install Node.js, which makes it easy to change the version of Node.js per project.

## Pull Request Submission Guidelines

Before you submit your Pull Request, consider the following guidelines:

* First check whether there is an open Issue for what you will be working on. If there is not, open one up by going through the Issue Submission Guidelines, including links to _related_ Issues found for context.
* Search for an open or closed Pull Request that relates to your submission. You don't want to duplicate effort, and you also want to include links to _related_ Pull Requests found for context.
* Make your changes in a new git branch:

```sh
git checkout -b <YOUR_USERNAME>/<ISSUE_NUMBER>/<SHORT_DESCRIPTION> main

// example: git checkout -b irmerk/75/readme-typos main
```

* Create your patch commit, **including appropriate test cases**.
* Commit your changes using descriptive commit messages that follows our Commit Guidelines.
* Pull Request titles should follow the same Commit Guidelines.
* When approved and ready to merge, a Pull Request should be squashed down to a single buildable commit and merged into `main`.


## Commit Guidelines

We have very precise rules over how our git commit messages should be formatted. This leads to **more readable messages** that are easy to follow when looking through the **project history** and **git logs**.

### Commit Message Format
Each commit message consists of a **type**, **scope**, **subject**, and **footer**. This is the format:

```shell
<TYPE>(<SCOPE>): <SUBJECT> #<FOOTER>
```

This allows the message to be easier to read on GitHub as well as in various git tools. Some examples:

```md
feat(core): add submit endpoint #559            // feature for core that will add a submission endpoint, from issue #559
fix(server): correct typo in readme #274        // fix for server that will correct typo in readme, from issue #274
chore(github): migrate ci/cd to gh actions #4   // chore for github that will migrate ci/cd to gh actions, from issue #4
docs(README): add interaction test script       // docs for README that will add interaction test script, from no issue
```

### Type
Must be one of the following:

* **`feat`**: A new feature
* **`fix`**: A bug fix
* **`docs`**: Documentation only changes
* **`style`**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* **`refactor`**: A code change that neither fixes a bug nor adds a feature
* **`perf`**: A code change that improves performance
* **`test`**: Adding missing or correcting existing tests
* **`chore`**: Changes to the build process or auxiliary tools and libraries such as documentation generation

### Scope
The scope will be specifying the place of the commit change; the focal point of new code or best description for where changes can be found.

You can use `*` when the change affects more than a single scope.

### Subject
The subject contains a succinct description of the change:

* the subject should finish a sentence of "*if merged, this commit will _____*"
* use the imperative, present tense: "change" not "changed" nor "changes"
* don't capitalize the first letter
* kept under 50 characters
* no period (`.`) at the end

### Footer
The footer should contain reference GitHub Issues that this commit addresses.

[discord]: https://discord.gg/7skRJ9nBxn
[support-email]: mailto:support@bookwormreads.co

[git]: http://git-scm.com/
[git-setup]: https://help.github.com/en/articles/set-up-git
[node]: https://nodejs.org/en/
[nvm]: https://github.com/creationix/nvm
[nvm-windows]: https://github.com/coreybutler/nvm-windows

[lang]: inclusive-language.md

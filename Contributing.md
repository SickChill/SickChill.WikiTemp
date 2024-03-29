### Questions about SickChill?

To get your questions answered, please ask on the [sickchill discord](https://discord.gg/FXre9qkHwE)

# Contributing to SickChill

1. [Getting Involved](#getting-involved)
2. [How To Report Bugs](#how-to-report-bugs)
3. [Tips For Submitting Code](#tips-for-submitting-code)

## Getting Involved

There are a number of ways to get involved with the development of SickChill. Even if you've never contributed code to an Open Source project before, we're always looking for help identifying bugs, cleaning up code, writing documentation and testing.

The goal of this guide is to provide the best way to contribute to the official SickChill repository. Please read through the full guide detailing [How to Report Bugs](#how-to-report-bugs).

## Discussion

If you think you've found a bug please report it on [discord](https://discord.gg/FXre9qkHwE), where you will find most of the sickchill dev team.

## How to Report Bugs

### Make sure it is a SickChill bug

Many bugs reported are actually issues with the user mis-understanding of how something works (there are a bit of moving parts to an ideal setup) and most of the time can be fixed by just changing some settings to fit the users needs.

If you are new to SickChill, it is usually a much better idea to ask for help first in the [sickchill discord](https://discord.gg/FXre9qkHwE). You will get much quicker support, and you will help avoid tying up the SickChill team with invalid bug reports.

### Try the latest version of SickChill

Bugs in old versions of SickChill may have already been fixed. In order to avoid reporting known issues, make sure you are always testing against the latest build/source. Also, we put new code in the `develop` branch first before pushing down to the `master` branch (which is what the binary builds are built off of).

### Reporting the issue

If the above steps fail and you are sure its a bug, issues are tracked in the [SickChill issue tracker](https://github.com/SickChill/SickChill).

## Tips For Submitting Code

### Code

**ALWAYS follow SickChill [Coding Standards](https://github.com/SickChill/sickchill.github.io/wiki/SickChill-Coding-Standards)**

Review regularly as they are subject to change and submissions will not be accepted until they meet our guidelines.

**NEVER write your patches to the master branch** - it gets messy (I say this from experience!)

**ALWAYS USE A "TOPIC" BRANCH!**

Personally I like the `branch-feature_name` format that way its easy to identify the branch and feature at a glance. Also please make note of any issue number in the pull commit so we know what you are solving (it helps with cleaning up the related items later).

#### Reporting

Please follow these guidelines before reporting a bug:

1. **Update to the latest version** &mdash; Check if you can reproduce the issue with the latest version from the `develop` branch.

2. **Use the search on SickChill** &mdash; check if the issue has already been reported. If it has been, please comment on the existing issue.

3. **Provide a means to reproduce the problem** &mdash; Please provide as much details as possible, e.g. SickChill log files (obfuscate apikey/passwords), browser and operating system versions, how you started SickChill, and of course the steps to reproduce the problem.

### Pull requests

[Pull requests](https://help.github.com/articles/using-pull-requests) are welcome and the preferred way of accepting code contributions.

Please follow these guidelines before sending a pull request:

1. Update your fork to the latest upstream version.

2. Use the `develop` branch to base your code off of. Create a topic-branch for your work. We will not merge your 'dev' branch, or your 'master' branch, only topic branches, coming from dev are merged.

3. Follow the coding conventions of the original repository. Do not change line endings of the existing file, as this will rewrite the file and loses history.

4. Keep your commits as autonomous as possible, i.e. create a new commit for every single bug fix or feature added.

5. Always add meaningful commit messages. We should not have to guess at what your code is supposed to do.

6. One pull request per feature. If you want multiple features, send multiple PR's

Please follow this process; it's the best way to get your work included in the project:

- [Fork](http://help.github.com/fork-a-repo/) the project, clone your fork,
  and configure the remotes:

```bash
   # clone your fork of the repo into the current directory in terminal
   git clone git@github.com:<your username>/SickChill.git
   # navigate to the newly cloned directory
   cd SickChill
   # assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/SickChill/SickChill.git
```

- If you cloned a while ago, get the latest changes from upstream:

  ```bash
  # fetch upstream changes
  git fetch upstream
  # make sure you are on your 'master' branch
  git checkout master
  # merge upstream changes
  git merge upstream/master
  ```

- Make sure that your develop branch is up to date:

  ```bash
  # Switch to the develop branch
  git checkout develop
  # Pull down any updates
  git pull
  ```

- Create a new topic branch to contain your feature, change, or fix:

  ```bash
  git checkout -b <topic-branch-name> develop
  ```

- Commit your changes in logical chunks. or your pull request is unlikely
  be merged into the main project. Use git's
  [interactive rebase](https://help.github.com/articles/interactive-rebase)
  feature to tidy up your commits before making them public.

- Push your topic branch up to your fork:

  ```bash
  git push origin <topic-branch-name>
  ```

- [Open a Pull Request](https://help.github.com/articles/using-pull-requests) with a
  clear title and description.

## Code guidelines

Read and follow the [SickChill Coding Standards](https://github.com/SickChill/sickchill.github.io/wiki/SickChill-Coding-Standards). Review these regularly as they are subject to change and code will not be accepted if it does not adhere to the standards.

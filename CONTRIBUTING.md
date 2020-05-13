# Contributing to CircuitVerse
[Back to `README.md`](README.md)

Thanks for checking out our contribution guide. We greatly appreciate any work contributed, no matter how small!

## How to Contribute
When you are ready to start work on an issue:

- Let us know by leaving a comment on the issue. (Also let us know later if you are no longer working on it.)
- Once you are assigned the issue (or once you have claimed the issue) only then proceed to make the Pull Request. This will help avoid multiple PRs pertaining to the same issue.

If you don't see your idea listed, do one of the following:
* **If your contribution is minor,** such as a typo fix, open a pull request.
* **If your contribution is major,** such as a new feature/enhancement, start by opening an issue first. That way, other people can be also involved in the discussion before you do any work.

## Version control branching
- Always make a new branch for your work, no matter how small. This makes it easy for others to take just that one set of changes from your repository, in case you have multiple unrelated changes floating around.

  * Don’t submit unrelated changes in the same branch/pull request! The maintainer shouldn’t have to reject your awesome bugfix because the feature you put in with it needs more review.
- Base your new branch off of the appropriate branch on the main repository:

  * Bug fixes should be based on the branch named after the **oldest supported release line the bug affects**.

     * Bug fixes requiring large changes to the code or which have a chance of being otherwise disruptive, may need to base off of master       instead.
  * New features should branch off of the **‘master’** branch.

     * Note that depending on how long it takes for the dev team to merge your patch, the copy of master you worked off of may get out of date! If you find yourself ‘bumping’ a pull request that’s been sidelined for a while, make sure you **rebase or merge to latest master to ensure a speedier resolution**.

## Pull Request Process

1. Create a branch. For example, if you are going to work on issue number #44 (which is, say, a new feature for ‘forgot password’ management):

        git checkout -b forgot-password#44

    This both creates and checks out that branch in one command.  
    The feature name should provide a (short) description of the issue.

2. Update the README.md with details of changes to the interface, this includes new environment variables, exposed ports, useful file locations and container parameters.
   
3. Develop the feature and push it to your local repo.
   
4. Create Pull Request (PR). Make sure to comment the issue that your PR is supposed to solve.

## Community
Discussions about CircuitVerse issues and features take place on the repository's [Issues](https://github.com/CircuitVerse/CircuitVerse/issues) and [Pull Requests](https://github.com/CircuitVerse/CircuitVerse/pulls) sections. Anybody is welcome to join these conversations. See the [README](README.md) for more information on communication channels.

## Code of Conduct

### Our Pledge

In the interest of fostering an open and welcoming environment, we as
contributors and maintainers pledge to making participation in our project and
our community a harassment-free experience for everyone, regardless of age, body
size, disability, ethnicity, gender identity and expression, level of experience,
nationality, personal appearance, race, religion, or sexual identity and
orientation.

### Our Standards

Examples of behavior that contributes to creating a positive environment
include:

* Using welcoming and inclusive language
* Being respectful of differing viewpoints and experiences
* Gracefully accepting constructive criticism
* Focusing on what is best for the community
* Showing empathy towards other community members

Examples of unacceptable behavior by participants include:

* The use of sexualized language or imagery and unwelcome sexual attention or
advances
* Trolling, insulting/derogatory comments, and personal or political attacks
* Public or private harassment
* Publishing others' private information, such as a physical or electronic
  address, without explicit permission
* Other conduct which could reasonably be considered inappropriate in a
  professional setting

### Our Responsibilities

Project maintainers are responsible for clarifying the standards of acceptable
behavior and are expected to take appropriate and fair corrective action in
response to any instances of unacceptable behavior.

Project maintainers have the right and responsibility to remove, edit, or
reject comments, commits, code, wiki edits, issues, and other contributions
that are not aligned to this Code of Conduct, or to ban temporarily or
permanently any contributor for other behaviors that they deem inappropriate,
threatening, offensive, or harmful.

## Contributors
### Financial Contributors

Becoming a [financial contributor](https://opencollective.com/CircuitVerse/contribute) help us sustain our community and platform.

#### Individuals
<a href="https://opencollective.com/CircuitVerse"><img src="https://opencollective.com/CircuitVerse/individuals.svg?width=890" alt="Individual financial contributors"></a>

#### Organizations
Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/CircuitVerse/contribute)]

<a href="https://opencollective.com/CircuitVerse/organization/0/website"><img src="https://opencollective.com/CircuitVerse/organization/0/avatar.svg" alt="Organization 1"></a>
<a href="https://opencollective.com/CircuitVerse/organization/1/website"><img src="https://opencollective.com/CircuitVerse/organization/1/avatar.svg" alt="Organization 2"></a>
<a href="https://opencollective.com/CircuitVerse/organization/2/website"><img src="https://opencollective.com/CircuitVerse/organization/2/avatar.svg" alt="Organization 3"></a>
<a href="https://opencollective.com/CircuitVerse/organization/3/website"><img src="https://opencollective.com/CircuitVerse/organization/3/avatar.svg" alt="Organization 4"></a>
<a href="https://opencollective.com/CircuitVerse/organization/4/website"><img src="https://opencollective.com/CircuitVerse/organization/4/avatar.svg" alt="Organization 5"></a>
<a href="https://opencollective.com/CircuitVerse/organization/5/website"><img src="https://opencollective.com/CircuitVerse/organization/5/avatar.svg" alt="Organization 6"></a>
<a href="https://opencollective.com/CircuitVerse/organization/6/website"><img src="https://opencollective.com/CircuitVerse/organization/6/avatar.svg" alt="Organization 7"></a>
<a href="https://opencollective.com/CircuitVerse/organization/7/website"><img src="https://opencollective.com/CircuitVerse/organization/7/avatar.svg" alt="Organization 8"></a>
<a href="https://opencollective.com/CircuitVerse/organization/8/website"><img src="https://opencollective.com/CircuitVerse/organization/8/avatar.svg" alt="Organization 9"></a>
<a href="https://opencollective.com/CircuitVerse/organization/9/website"><img src="https://opencollective.com/CircuitVerse/organization/9/avatar.svg" alt="Organization 10"></a>

### Code Contributors

This project only exists thanks to all the people who have [contributed]((CONTRIBUTING.md)).
<a href="https://github.com/CircuitVerse/CircuitVerse/graphs/contributors"><img src="https://opencollective.com/CircuitVerse/contributors.svg?width=890&button=false" alt="Code contributors" /></a>

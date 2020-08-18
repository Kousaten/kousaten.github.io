# Contributing

We are happy to receive your contributions and you have to follow some rules to keep the project tidy

Read the following carefully please, we will refuse all the non-compliant pull requests cruely

Of course, if you really don't follow the rules, we will give you a guide to teach you make your pull request compliant

Now, let's see the rules!

## Basic Workflow

> Tips: Text surrounded by angle brackets changable variable

### Workflow for Kousaten "writers"

- Use `git clone https://github.com/Kousaten/<repository_name>` to clone the repository to your disk
- Open your terminal emulator and open the directory with the command `cd`
- Create a new branch using `git branch <branch_name>`
- Change to the branch using `git checkout <branch_name>`
- Start writing code
- Add, Commit, Push your code
- Open a new pull request

### Workflow for Everyone

- Fork the project you want to contribute
- Clone the forked repository to your disk
- Create a new branch using `git branch <branch_name>`
- Change to the branch using `git checkout <branch_name>`
- Start writing code
- Add, Commit, Push your code
- Open a new pull request in the forked repository

### Things to Pay Attention

- [How to name a branch?](Contributing?id=branch-name-style)
- [How to write code compliant?](Contributing?id=code-style)
- [How to write commit messages?](Contributing?id=commit-message-style)
- [How to open a new pull request correctly?](Contributing?id=pull-request-style)

## Styling

### Branch Name Style

You need to submit a Pull Request (PR) from a new branch with a name related to the changes. Pull Request from master branch will be rejected. This is because when you open a Pull Request from a branch, you can still update the Pull Request by committing and pushing to the branch

Here's the name style for branches:

- name of new features' branch should be starts with `feature/`.
  For example, `feature/login` means the branch added login feature. `feature/optimize_login` means the branch optimized login feature

- name of bug's fixing branch should be starts with `fix/`.
  For example, `fix/login` means the branch fixed the bugs in login feature

- changes of documents' branch should be starts with `docs/`
  For example, `docs/style` means the branch changed the text style of documents

### Code Style

We're sorry but we don't have a standard of codes now, you can follow the generic style of the programming language

### Commit Message Style

You should make the changes in the commit clear, because it's going to generate changelogs using the commit messages

Commit message should follow the [AngularJS Git Commit Message Conventions](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#heading=h.uyo6cb12dt6w) as the following:

> `<type>(scope): <subject>`
>
> // blank line
>
> `<body>`
>
> // blank line
>
> `<footer>`

In most instances, commit message should only have the first line. the second and the third line is optional

### Pull Request Style

#### Pull Request Title

- If there's only one commit in the branch, pull request title can be the same as the last commit message or can follow the following rules
- If there's many commits in the branch, pull request title writing should follow the following rules:
  - Pull request title should be starts with the first half of the branch name, such as `feature`, `fix`, `docs` and so on
  - Pull request title should be ends with the specific change of the branch, such as `login`, `style`, sometimes it can be the second half of the branch name

#### Pull Request Description

Pull Request Description is for that the reviewers can understand your changes more clearly. This part can't be empty

Here's a Template of a Pull Request Description
> The original author of the template is [BobAnkh](https://github.com/BobAnkh)
> Original link is [here](https://github.com/BobAnkh/LinuxBeginner/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
> The template is under Apache 2.0 License

```markdown

## Description
<!--- Why is this change required? What problem does it solve? -->
<!--- Describe your changes in detail here to communicate to the maintainers why this pull request should be accepted -->
<!--- Describe your technology stack here if not a documentation update -->
<!--- Tasklist format is recommended for all pull requests and is required for all draft pull requests. You can couple your description with the tasklist -->
<!--- If it fixes an open issue, please link to the issue here in the last line. -->

## How Has This Been Tested
<!--- Please describe in detail how you tested your changes locally -->
<!--- Include details of your testing environment, and the tests you ran to -->
<!--- For example, markdown files should pass markdownlint locally according to the rules -->
<!--- See how your change affects other areas of the code, etc. -->

## Screenshots(optional)
<!--- If Screenshots is not necessary or not available in this pull request, you can delete this section -->
<!--- Changes including html and css are required to have screenshots -->

## Types of changes
<!--- What types of changes does your code introduce? -->
<!--- Only left the line that best describes this pull request -->
- Bug fix (non-breaking change which fixes an issue)
- New feature (non-breaking change which adds functionality)
- Documentation (non-breaking change which updates documentation)
- Breaking change (fix or feature that would cause existing functionality to change)
- Code style (formatting, renaming)
- Refactoring (no functional changes, no api changes)
- Other (please describe here):

## Checklist
<!--- Go over all the following points, and put an `x` in all the boxes that apply. -->
<!--- If you're unsure about any of these, don't hesitate to ask. We're here to help! -->
- [ ] Code follows the code style of this project.
- [ ] Changes follow the **CONTRIBUTING** guidelines.
- [ ] Update necessary documentation accordingly.
- [ ] Lint and tests pass locally with the changes.
- [ ] Check issues and pull requests first. You don't want to duplicate effort.

## Other information
<!--- Be empty or write somthing you want -->

`

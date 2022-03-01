# Workflows

[<< Precourse](https://gitub.com/hackyourfuturebelgium/precourse) | Workflows |
[Agile Development >>](../agile-development/README.md)

> “I'm not a great programmer; I'm just a good programmer with great habits.”
>
> - [Kent Beck](https://en.wikiquote.org/wiki/Kent_Beck)

Learn the skills required to work a collaborative software project using only
Markdown. Limiting your projects to Markdown lets you focus on the big picture
without getting distracted by more challenging code.

- [Learning Objectives](#learning-objectives): what you can expect to learn from
  studying this material
- [Suggested Study](./suggested-study.md): Helpful links for this module, useful
  but not required.
- [Deliverables](./deliverables): Projects to practice applying the learning
  objectives in context
- [Lesson Plans](./lesson-plans): A few ideas for running lessons around this
  material.
- [Setting Up](#setting-up)
- [Study Tips](#study-tips)
- [Code Quality Scripts](#code-quality-scripts)

## Learning Objectives

<details>
<summary>Priorities: 🥚, 🐣, 🐥, 🐔 (click to learn more)</summary>
<br>

There is a lot to learn in this repository. If you can't master all the material
at once, that's expected! Anything you don't master now will always be waiting
for you to review when you need it. These 4 emoji's will help you prioritize
your study time and to measure your progress:

- 🥚: Understanding this material is required, it covers the base skills you'll
  need for this module and the next. You do not need to finish all of them but
  should feel comfortable that you could with enough time.
- 🐣: You have started all of these exercises and feel you could complete them
  all if you just had more time. It may not be easy for you but with effort you
  can make it through.
- 🐥: You have studied the examples and started some exercises if you had time.
  You should have a big-picture understanding of these concepts/skills, but may
  not be confident completing the exercises.
- 🐔: These concepts or skills are not necessary but are related to this module.
  If you are finished with 🥚, 🐣 and 🐥 you can use the 🐔 exercises to push
  yourself without getting distracted from the module's main objectives.

---

</details>

### [0. Local Development Without Git](./0-local-development-without-git)

Practice the foundational workflows of software development by learning to write
Markdown locally on your own computer using Visual Studio Code (VSCode), the
Command Line Interface (CLI), and NPM scripts to automate your code's quality
(formatting, linting and spell checking).

- [ ] 🥚 **Folder Structures**: You can explain how files and folders are stored
      in your computer and can find, open or create files in your computer
      without using the Command Line Interface.
- 🥚 **Command Line Interface (CLI)**: In a Unix shell you can ...
  - [ ] open a new terminal window
  - [ ] navigate up and down directories using `cd`
  - [ ] list the contents of a directory using `ls`
  - [ ] view the contents of a file using `cat`
  - [ ] create new files using `touch`
  - [ ] create new folders using `mkdir`
- [ ] 🥚 **Markdown**: You can write a document in Markdown with no syntax
      mistakes that renders into a well-formatted document.
- 🥚 **VSCode**: You can complete these workflows in VScode, and can use
  keyboard shortcuts to complete them all:
  - [ ] Opening a repository in a new window
  - [ ] Opening the VSCode terminal
  - [ ] Adding a new file
  - [ ] Adding a new folder
  - [ ] Deleting a file
  - [ ] Deleting a folder
  - [ ] Previewing a Markdown File
  - [ ] Formatting a Markdown document
- [ ] 🥚 **READMEs**: You can write a README file that describes the project you
      are working on, why it's helpful, and how someone can use it.
- 🥚 **NPM**: You can use NPM commands to verify your code's quality, this
  includes ...
  - [ ] using `npm install` to install a project's dependencies
  - [ ] reading a `package.json` file to find which scripts are available for
        the project
  - [ ] use `npm run <script>` to execute an npm script
- 🥚 **Formatting Code**: You can use Prettier to make sure all the code in your
  project is well-formatted:
  - [ ] You can use the Prettier VSCode extension to format a document while you
        are writing it
  - [ ] You can use `npm run format` to format all of the documents in your
        project
  - [ ] You can use `npm run format:check` to make sure all files are
        well-formatted
- 🥚 **Linting Code**: You can ...
  - [ ] use `npm run lint:md` to check all Markdown files in your folder for
        linting mistakes
  - [ ] you can fix all linting mistakes reported by `npm run lint:md`
- 🥚 **Spell Check**: You can ...
  - [ ] use the Code Spell Checker VSCode extension to correct spelling mistakes
        in your Markdown documents while you are writing
  - [ ] use `npm run spell-check` to check the spelling in all the files of your
        project
  - [ ] update `.cspell.json` to add words that should be allowed in your
        project
- 🥚 **File and Folder Naming Conventions**: You can ...
  - [ ] identify and follow the naming conventions for the project you are
        working on.
  - [ ] use `npm run lint:ls` to check that all files and folders follow the
        project's naming conventions.
  - [ ] you can correct any file and folder names to make them match the project
        conventions.
- [ ] 🐣 **File Extensions**: You can identify all of the languages covered at
      HYF and give the correct file extension. You don't need to know the
      languages, just recognize them.
- [ ] 🐣 **Touch Typing**: You can write a Markdown file without looking at your
      keyboard to find any letters, numbers or special characters. (slowly is
      ok!)

### [1. Local Development With Git](./1-local-development-with-git)

Practice using Git to save and organize your development process. You will learn
how you can use Git to go back to previous versions of your project, and to work
on different changes in parallel.

- 🥚 **Git**: Using the CLI you can ...
  - [ ] Initialize a new git repository with `git init`
  - [ ] stage changes using `git add <path>`
  - [ ] commit changes using `git commit -m <message>`
  - [ ] display your repository's git history using `git log`
  - [ ] create a new branch using `git branch <branch-name>`
  - [ ] check out a branch using `git checkout <branch-name>`
  - [ ] create a new branch and check it out using
        `git checkout -b <branch-name>`
  - [ ] merge changes from one branch to another using `git merge <branch-name>`
  - [ ] return to a previous version of your project with `git log` and
        `git checkout <commit-hash>`
  - [ ] stash and retrieve uncommitted changes with `git stash` and `git pop`
- 🥚 **`.gitignore`**: You can use a `.gitignore` file to describe which files
  you don't want included in your git history.
- 🥚 **VSCode**: You can ...
  - [ ] use the _Git Graph_ extension to to visualize your repo's commit history
  - [ ] use the _Git Lens_ extension to investigate your repository's commit
        history
  - [ ] explain how the file tree in VSCode can show you which files have
        uncommitted changes
- [ ] 🥚 **Atomic Commits**: You can save your development progress using small
      commits with clear and helpful message.
- [ ] 🐣 **Feature Branches**: You can organize your development process using
      branches. You can create a new branch for each part of your project and
      merge those changes to `main` when they are finished.

### [1. Local/Remote Development](./2-local-remote-development)

Learn how you can connect your local Git repositories with a GitHub repository
to add more structure to your development process and to share your projects.

- 🥚 **Licenses**: You can ...
  - [ ] explain why it's important to include a license for your code on GitHub
  - [ ] choose a license for your projects that matches how you want others to
        use your code
- 🥚 **GitHub**: You can ...
  - [ ] create new repository on GitHub
  - [ ] write a description for your repository
  - [ ] turn on GitHub Pages
  - [ ] configure your repository to block pushing to `main`
  - [ ] configure your repository to block merging to `main` until Continuous
        Integration (CI) checks have passed
- 🥚 **Git Remote/Local Connection**: You can ...
  - [ ] clone a remote repository to your computer
  - [ ] initialize a new repository locally and connect it to an empty remote
        repository
  - [ ] `push` and `pull` changes between remote & local branches
- [ ] 🥚 **Pull Requests**: You can create a pull request between two branches
      in your repository and merge changes without causing any conflicts.
- [ ] 🥚 **PR templates**: You can use a PR template to add a checklist to all
      of your PRs so you are sure the code is great before merging to `main`.
- [ ] 🥚 **Continuous Integration**: You can use GitHub Actions to check your
      code's quality before merging a pull request to the `main` branch.
- [ ] 🐣 **Local/Remote Branching Workflow**: You can use a branching workflow
      that keeps mistakes away from the `main` branch and prevents conflicts
      from happening in GitHub. For each contribution to the project you can ...
  1. Check out a new local branch and write your code
  2. Check out `main` on your local machine
  3. Pull changes from remote `main` to local `main`
  4. Merge changes locally from `main` to your new branch
     - Fix any conflicts on your new branch before pushing!
  5. Format and lint your code
  6. Push your new local branch to your remote repository
  7. Open a Pull Request from the new branch to `main`
     - Go through the PR's checklist to make sure everything is correct
     - Make sure all CI checks pass!
  8. Merge your new remote branch to `main`
     - You can delete the branch after it's merged if you want to

### [3. Remote Collaboration](./3-remote-collaboration)

Learn how to collaborate with a group on a single project hosted in a GitHub
repository. Practice using GitHub's project management features to organize your
group's tasks and to double-check your project's code quality.

- [ ] 🥚 **Contributor Guidelines**: Your group can define contributor
      guidelines that describes how everyone can add their work to the project.
- [ ] 🥚 **Code of Conduct**: Your group can write a code of conduct for your
      project that describes how everyone should communicate and what behavior
      is considered unproductive.
- [ ] 🥚 **Repository Contributors**: You can add group members as collaborators
      in a repository.
- [ ] 🥚 **Issue Templates**: Your group can use issue templates to make sure
      all issues are complete and relevant to the project. in your repository
      and merge changes without causing any conflicts.
- [ ] 🥚 **Code Review**: You can use the PR Template and CI checks to review
      another group member's code before merging it to `main`.
- 🐣 **GitHub Project Management**: You can ...
  - [ ] use issues to define tasks in a group project. Each issue should have a
        helpful title, complete description, and helpful labels.
  - [ ] use a Project Board to organize a project's issues
  - [ ] claim issues and track your progress with the project board
  - [ ] link a PR to your claimed issue
  - [ ] assign someone to review your PR
  - [ ] use GitHub code review features to discuss your code with your reviewer

### [4. Open Source Development](./4-open-source-development)

Explore the wider world of Open Source software by learning how a community of
independent developers write and maintain the code we all rely on.

- [ ] 🥚 **Finding Issues**: You can read through an open source project's
      issues and determine if there is one you can help with.
- [ ] 🥚 **Opening Issues**: You can open a helpful issue in an open source
      repository, following their contributor guidelines and code of conduct.
- [ ] 🥚 **Forking & PRS**: You can create a fork of an open source project and
      send a PR to the primary repository.

[TOP](#workflows)

---

## Setting Up

> You will need
> [NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
> installed on your computer to study this material

1. Clone this repository:
   - using SSH:
     `git clone --depth 1 git@github.com:HackYourFutureBelgium/workflows.git`
2. navigate to the cloned repository
   - `cd workflows`
3. Install dependencies:
   - `npm install`

> It's highly recommended that you use either Linux or Mac. If you have a
> Windows computer you can either dual-boot your computer or install a virtual
> machine.

[TOP](#workflows)

---

## Study Tips

<details>
<summary>expand/collapse</summary>
<br>

- Don't rush, understand! Programming is hard.
  - The examples and exercises will still be there to study later.
  - It's better to fail tests slowly and learn from your mistakes than to pass
    tests quickly and not understand why.
- Don't skip the examples! Understanding and experimenting with working code is
  a very effective way to learn programming.
- Write lots of comments in the examples and exercises. The code in this
  repository is yours to study, modify and re-use in projects.
- Practice
  [Pair Programming](https://home.hackyourfuture.be/students/study-tips/pair-programming):
  two people, one computer.
- Take a look through the
  [Learning From Code](https://home.hackyourfuture.be/students/study-tips/learning-from-code)
  guide for more study tips

### Study Board

Creating a project board on your GitHub account for tracking your study at HYF
can help you keep track of everything you're learning. You can create the board
at this link: `https://github.com/your_user_name?tab=projects`.

These 4 columns may be helpful:

- **todo**: material you have not studied yet
- **studying**: material you are currently studying
- **to review**: material you want to review again in the future
- **learned**: material you know well enough that you could help your classmates
  learn it

</details>

[TOP](#workflows)

---

## Code Quality Scripts

<details>
<summary>expand/collapse</summary>
<br>

This repository comes with some scripts to check the quality of this code. You
can run these scripts to check the code provided by HYF, and to check the code
you write when experiment with the examples and complete the exercises.

### `npm run format`

This script will format all of the code in this repository making sure that all
the indentations are correct, the code is easy to read, and letting you know if
there are any syntax errors.

### `npm run format:check`

Checks the formatting of all files in the repository and throws an error if any
files are not well-formatted.

### `npm run spell-check`

This script will check all of the files in your repository for spelling
mistakes. Spelling is not just a detail, is important! Good spelling helps
others read and understand your programs with less effort.

`spell-check` is not so clever though, it doesn't have _all_ possible words in
it's dictionary and it won't know if you _wanted_ to spell a word incorrectly.
If you think one of it's "Unknown word"s is not a problem, you can either ignore
the suggestion or add the word to the `"words": [ ... ],` list in
[.cspell.json](./.cspell.json).

### `npm run lint:md`

This script will [lint](https://en.wikipedia.org/wiki/Lint_%28software%29) all
the Markdown files in this repository, checking for syntax mistakes and other
bad practices. Fixing linting errors will help you learn to write better code by
pointing out your mistakes _before_ they cause problems in your program.

Some linting errors will take some practice to understand and fix, but it will
be a good use of time.

### `npm run lint:ls`

This script will [lint](https://en.wikipedia.org/wiki/Lint_%28software%29) the
names of all files and folders in the project to check that they follow the
project naming convention
([kebab-case](https://betterprogramming.pub/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841)).

</details>

[TOP](#workflows)

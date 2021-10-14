# Workflows

Examples, exercises and guides for the
[Workflows module](https://home.hackyourfuture.be/curriculum/workflows)

## Getting Started

> You will need
> [NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
> installed on your computer to study this material

1. Clone this repository:
   - using SSH: `git clone git@github.com:HackYourFutureBelgium/workflows.git`
2. navigate to the cloned repository
   - `cd workflows`
3. Install dependencies:
   - `npm install`

---

## Materials

- 🥚 **[./guides](./guides)**: This folder contains short videos showing how to
  do many of the little skills and habits you need to learn in this module.
  Things like inspecting an element in the DOM, navigating a folder system from
  the Command Line Interface, and creating a new branch with Git.
- 🥚 **[./file-extensions](./file-extensions)**: Some guidance and exercises for
  recognizing the different languages you will learn at HYF. You will need to
  figure out what language is written in each file and add the correct file
  extension.
- 🥚 **[./markdown](./markdown)**: A few example files showing different
  formatting options available in Markdown.
- 🥚 **[./project-starter](./project-starter)**: Starter materials for the
  HTML+CSS group project.

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

### Priorities

If you can't finish all the material in this repository, that's expected!
Anything you don't finish now will always be waiting for you to review when you
need it. These 4 emoji's will help you prioritize your study time and to measure
your progress:

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

### Hashtags

There's so many examples and exercises in this repository, it's easy to forget
of what you still need to finish or what you want to review again. Luckily
VSCode is really good at searching through folders of code.

You can write hashtags in your comments while you're studying, then search for
those hashtags later so you don't miss anything. Here's some ideas:

- `// #todo, still a few blanks left` - search for `#todo` in Study Lenses or
  VScode to find all the exercises you still need to study
- `// #review, coercion is confusing this again next week` - search for
  `#review` to find the files you need to study again
- ... anything goes! Find the hashtags that work for you

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

### `npm run lint:css`

Just like `lint:md`, but for `.css` files. This script will lint all of the CSS
files in this repository, letting you know if there are any syntax errors or bad
practices.

### `npm run validate:html`

Validating HTML is sort of like linting, but a little more involved. When you
validate an HTML file the script will not only check the source code, but
actually open the file in a _headless browser_ and check the website for
mistakes.

You can think of a headless browser as a normal browser, but one where you can't
see the web page. They're generally used for testing and validation when it's
not important that a user can interact directly with the web page

</details>

[TOP](#workflows)

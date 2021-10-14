# Issues

This is a suggestion for the issues you can use to track your progress. You will
want to create these issues and track them on your repository's project board.

Feel free to change these or add new issues if that works better for your team.

---

## Planning Milestone

Tasks related to planning your project will all be placed under the `planning`
milestone. Below are some of the planning tasks, but not all! Your group will
certainly come up with new tasks or ideas for planning. All of these can be
added to issues under the `planning` milestone.

### Communication Plan

An issue to discuss your group's schedule and communications plan, this can be
linked to PRs that contribute to the `/planning/communication.md` file.

- **Labels**: `communication`, `type: planning`

### Backlog

An issue to discuss the project backlog, this can be linked to PRs that
contribute to the `/planning/backlog.md` file.

- **Labels**: `backlog`, `type: planning`

### Design

An issue to discuss the project's design, this can be linked to PRs that
contribute to the `/planning/design.md` file. In simpler projects like this the
goal of a design is to create a wireframe.

- **Labels**: `design`, `type: planning`

### Development Strategy

An issue to discuss the project's development strategy, this can be linked to
PRs that contribute to the `/planning/development-strategy.md` file. This first
project already has a starter development strategy, but your team may want to
make changes.

- **Labels**: `development strategy`, `type: planning`

Remember! The development strategy is a living document, it will change all the
time. You don't need to write a perfect one from the beginning. In Agile
Development it's expected that your plans will change as you build the project.
What matters is how well you adapt to these changes, not how perfect your plan
is.

---

## Development Milestones

You'll be learning to develop your website based on _user stories_. Your
_backlog_ will contain a big list of possible user stories organized by
priority. Each of these priorities will be a separate _milestone_ in your
project:

- `must have`: these are necessary for basic usability
- `should have`: will complete the user experience, but are not necessary
- `could have`: would be really cool ... if there's time

Each user story or _feature_ will have it's own label, and you may have more
than one issue for each user story! Imagine for example that you have already
merged code for the web page's header but then one of your group members notices
it does not work in Chrome. Your original issue will already be closed, so your
classmate can open a _new_ issue with the user story's label and suggest a fix
for browser compatibility.

### Must-Have Issues

Some tips to get you started creating issues from the development strategy. Feel
free to change these if your team wants to, it's just a starting suggestion:

<details>
<summary> Site Title: Interface </summary>
<br>

**Milestone**: `must have`

**labels**:

- `for: site title` (description: _"as a user can read the title of the page"_)
- `type: interface`
- `html`, `css`

**Issue Body**:

```markdown
The site needs a clear title that's easy to read at the top of the page.

Header with centered title

- [ ] HTML: a header element with the title
- [ ] CSS: a class to center the title
```

</details>
<details>
<summary> Introduction: Interface </summary>
<br>

**Milestone**: `must have`

**labels**:

- `for: introduction` (description: _"As a user I can read an introduction to
  this project"_)
- `type: interface`
- `html`, `css`

**Issue Body**:

```markdown
It should be clear what this project is for and what someone can expect from the
web page.

A body of text and links

- [ ] HTML: a section with some general information about the project
- [ ] CSS: a class to make the text look fancy
```

</details>
<details>
<summary> Main Info: Interface </summary>
<br>

**Milestone**: `must have`

**labels**:

- `for: main info` (description: _" "As a user I can learn about trees"_)
- `type: interface`
- `html`, `css`

**Issue Body**:

```markdown
There is a main text in the page with helpful info and links.

Header with centered title

- [ ] HTML: a section with some general information about the project
- [ ] HTML: a pretty list of links
- [ ] CSS: a class to format the list
```

</details>
<details>
<summary> Extra Info: Interface </summary>
<br>

**Milestone**: `must have`

**labels**:

- `for: extra info` (description: _" "As a user I can learn even more about
  trees"_)
- `type: interface`
- `html`, `css`

**Issue Body**:

```markdown
Some more links for students who want to go beyond the basics.

An aside with links for digging deeper.

- [ ] HTML: some helpful text and a reference link
- [ ] CSS: a class to position the aside
- [ ] CSS: a class to style the text
```

</details>

> PS. You'll learn more about what `type: interface` means in the Separation of
> Concerns module

---

## Retrospective Milestone

Your projects will always take more time than you have. It's not important that
you finish every project at HYF, what's important is that you try your best and
learn from your mistakes.

When it is time to submit the assignment what's important is that your team has
a good _retrospective_. This will be a document where your team goes over what
went well, what didn't go well, and what to do differently next time.

Issues in this milestone will be anything related reviewing, discussing, and
learning from what went well and what did not. There should also PRs to the
`/planning/retrospective.md` file where your group will collect all lessons
learned.

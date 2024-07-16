## Commit Message Format

Each commit message consists of a **header**, a **body**, and a **footer**. The header has a special format that includes a **type**, a **scope**, and a **subject**:

```
<type>(<scope>): <subject>
<BLANK LINE>

<body>
<BLANK LINE>
<footer>
```

The header is mandatory and the scope of the header is optional.

Example — `fix: remove unused dependency lodash.camelcase`

Any line of the commit message cannot be longer than 100 characters. This allows the message to be easier to read on GitHub as well as in various git tools.

#### Type
Must be one of the following:
- feat: A new feature.
- fix: A bug fix.
- docs: Documentation only changes.
style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc).
- refactor: A code change that neither fixes a bug nor adds a feature.
- perf: A code change that improves performance.
- test: Adding missing tests.
- chore: Changes to the build process or auxiliary tools and libraries such as documentation generation.
- ci: Changes to our CI configuration files and scripts.
- build: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm).
- revert: Reverts a previous commit.
- wip: Work in progress. Commit that may be removed later.

#### Scope
The scope is optional and could be anything specifying the place of the commit change. For example `nsis`, `mac`, `linux`, etc.

#### Subject
The subject contains a succinct description of the change:

- Use the imperative, present tense: change not changed nor changes.
- Don't capitalize the first letter.
- No dot (.) at the end.


#### Body
Just as in the subject, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with the previous behavior.

#### Footer
The footer should contain any information about Breaking Changes and is also the place to reference GitHub issues that this commit Closes.

Breaking Changes should start with the word BREAKING CHANGE: with a space or two newlines. The rest of the commit message is then used for this.

### Best Practices
- Write Meaningful Commit Messages: Ensure that each commit message clearly conveys what the change is and why it was made. This is crucial for maintaining a clear project history.
- Keep Commits Small: Each commit should represent a single logical change. This makes it easier to review changes and revert them if necessary.
- Use Branches: For each new feature or bug fix, create a new branch. This helps in keeping the main branch stable and allows for easier collaboration.
- Squash Commits: Before merging a feature branch into the main branch, consider squashing commits to ensure a clean and concise project history.
- Review Before Commit: Review your changes before committing. Ensure that your code adheres to the project's coding standards and passes all tests.
- Automate Testing: Set up automated tests to run on each commit to ensure that changes do not introduce new bugs.
- Follow a Consistent Style: Adhere to the established style guide for the project to maintain consistency across the codebase.

Ref
- FreeCodeCamp. (2022, March 2). How to write better Git commit messages. FreeCodeCamp. https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/
- Beams, C. (n.d.). How to write a Git commit message. Retrieved July 16, 2024, from https://cbea.ms/git-commit/
- 2my. (2021, October 30). Git conventional commits. 2my Blog. https://blog.2my.xyz/2021/10/30/git-conventional-commits/

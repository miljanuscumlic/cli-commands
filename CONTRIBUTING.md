# Contributing 

1. Fork the repository.
2. Clone forked repository and create a new branch.
3. Make changes to a single file of your choice e.g. `git-commands.md`.
4. Every file containing terminal commands has a header:

   | Command | Description | Note | Version | Docs |
   |:--- |:--- |:--- |:--- |:--- |

   **Command** column should be populated with the command string enclosed with two backtick characters e.g. `git add -A`.<br />

   In the best case scenario **Version** column should represent the software version that introduced particular command. If you don't know which version is that, or you don't want to look up for it just put the software version you have tested command with.<br />

   **Docs** column should be populated with the documentation link describing the command in question.
5. Sort all lines by the command string between the backticks. In vim lines could be sorted with the command ```:sort r /`[^`]*/```
6. Commit messages should be succinct, but while writing them follow these rules as much as possible: [The seven rules of the great Git commit message](https://chris.beams.io/posts/git-commit/#seven-rules)
7. Prepend a subject of a commit message with appropriate mark e.g. when contributing to a `git-commands.md` prepend it with `[git]`: `git commit -m "[git] Add salute to live long and prosper"`.
8. Put further clarifications of a commit changes if necessary at all inside a commit message description.
9. Submit Pull Request to the **develop** branch with description of changes.
10. We encourage you to add yourself to a list of all our contributors by commenting your pull request (or issue you have made) with: `@all-contributors please add @<github_username> for <contributions>`.<br />
   Most appropriate for `<contributions>` is `doc` because we are documenting the usage of the commands. Full documentation on all-contributors bot we are using for this purpose  can be found [here](https://allcontributors.org/docs/en/bot/usage).

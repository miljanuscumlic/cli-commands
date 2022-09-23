# Contributing 

1. Fork the repository.
2. Clone forked repository and create a new branch.
3. Decide which single file would you like to contribute to, and make a new branch. E.g. if you want to make a contribution to the `bash.md` make a branch from the `bash` branch of this repository.
4. Every file containing terminal commands has a header:

   | Command | Description | Note | Version | Docs |
   |:--- |:--- |:--- |:--- |:--- |

   **Command** should contain the command string enclosed with two backtick characters e.g. `git add <file_name>`. As can be seen in this example you can use metasymbols `<` and `>` as delimiters of a class name as it is called in the Backus–Naur form. Class name represents the class of objects that could be used in its place when writing actual command. Class name should be written in a `snake_case`. Every character outside the metasymbols `<` and `>` in an actual command is used as is.<br />
 
   **Description** should be written in the imperative form and in a `small case`. Descriptions should be clear and as concise as possible. <br />

   **Note** is optional and could contain additional clarification of a command, short warning of some edge cases, prerequisites, exceptions or something else. Should be written in a `small case`. <br />

   In the best case scenario **Version** should represent the software version that introduced particular command. If you don't know which version is that, or you don't want to look up for it just put the software version you have tested command with.<br />

   **Docs** column should be populated with the documentation link describing the command in question. If no apt link is available it could be left blank.
5. Sort all lines by the command string between backticks. In vim, lines could be sorted with the command ``:sort r /`[^`]*/``
6. Commit messages should be succinct, but while writing them follow these rules as much as possible: [The seven rules of the great Git commit message](https://chris.beams.io/posts/git-commit/#seven-rules)
7. Prepend a subject of a commit message with appropriate mark e.g. when contributing to the `git-commands.md` prepend it with `[git]`: `git commit -m "[git] Add salute to live long and prosper"`.
8. Put further clarifications of a commit changes inside a commit message description, if you feel it's necessary.
9. Submit a Pull Request with description of changes to the appropriate branch. E.g. if you made a branch from the `bash` branch, submit a Pull Request to the `bash` branch of the repository.
10. We encourage you to add yourself to the list of all our contributors by commenting your pull request with: `@all-contributors please add @<github_username> for <contributions>`.<br />
   The most appropriate value for `<contributions>` is `doc` because we are documenting the usage of commands. Full documentation on all-contributors bot which we are using for this purpose can be found [here](https://allcontributors.org/docs/en/bot/usage).

## Additional notes

It is a good practice to test how markdown file you are modifying looks like before you push your changes to the repository. Although the rendering isn't completely the same as on the github for this purpose you can use this [site](https://markdown-it.github.io/).

If you would like to start documenting commands for a tool or a program that doesn't yet have its `.md` file you are advised to start from the [template](https://github.com/miljanuscumlic/cli-commands/blob/master/template.md). Name the file by the tool you are documenting and place it in the `/commands` directory.

| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `gh alias set <alias_name> '<command>'` | create alias for the given command | command can have arguments designated with a dollar sign notation e.g. `$1` | 2.83.2 | [link](https://cli.github.com/manual/gh_alias_set) |
| `gh config get <key>` | get a value for the settings key | | 2.83.2 | [link](https://cli.github.com/manual/gh_config_get) |
| `gh config list` | list all confuration settings for github cli | | 2.83.2 | [link](https://cli.github.com/manual/gh_config) |
| `gh config set <key> <value>` | set a value for the settings key | e.g. `gh config set editor vim` | 2.83.2 | [link](https://cli.github.com/manual/gh_config_set) |
| `gh issue close <issue_number>` | close the issue of the given number | | 0.9 | [link](https://cli.github.com/manual/gh_issue_close) |
| `gh issue create` | create issue in interactive mode | interactively populate properties of the issue | 0.9 | [link](https://cli.github.com/manual/gh_issue_create) |
| `gh issue list` | list all the issues in the repository | by default it only lists open issues | 0.9 | [link](https://cli.github.com/manual/gh_issue_list) |
| `gh issue view <issue_number>` | view issue with the given number | | 0.9 | [link](https://cli.github.com/manual/gh_issue_view) |
| `gh pr checkout <pull_request_number>` | check out the pull request in git | | 0.9 | [link](https://cli.github.com/manual/gh_pr_checkout) |
| `gh pr create` | create pull request in interactive mode | command can also work non-interactively using flags | 0.9 | [link](https://cli.github.com/manual/gh_pr_create) |
| `gh pr diff` | look at the diff made with the pull request | | 0.9 | [link](https://cli.github.com/manual/gh_pr_diff) |
| `gh pr edit <pull_request_number>` | edit pull request in interactive mode | | 2.83.2 | [link](https://cli.github.com/manual/gh_pr_edit) |
| `gh pr list` | list all the pull request in the repository | by default it only lists open pull requests | 0.9 | [link](https://cli.github.com/manual/gh_pr_list) | 
| `gh pr merge <pull_request_number>` | interactively merge pull request with the given number | | 0.9 | [link](https://cli.github.com/manual/gh_pr_merge) |
| `gh pr status` | display information about pull requests of the current users or on the current branch | | 0.9 | [link](https://cli.github.com/manual/gh_pr_status) | 
| `gh pr view <pull_request_number>` | display information about given pull request | | 2.83.2 | [link](https://cli.github.com/manual/gh_pr_view) |
| `gh pr view <pull_request_number> --json commits` | display JSON fields corresponding to the commits containted in the given pull request | | 2.82.3 | |
| `gh pr view <pull_request_number> --json files --jq '.files.[].path'` | display file names of files' changed in the given pull request | | 2.82.3 | |
| `gh pr view <pull_request_number> -w` | open web github web page displaying given pull request | |  2.83.2 | [link](https://cli.github.com/manual/gh_pr_view) |
| `gh repo set-default` | set default repo in interactive mode | | 0.9 | [link](https://cli.github.com/manual/gh_repo_set-default) |
| `gh repo view -b <branch_name>` | display repository description and README version of a given branch | | 0.9 | [link](https://cli.github.com/manual/gh_repo_view) |

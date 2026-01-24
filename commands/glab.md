| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `glab mr update <merge_request_id> -t <title>` | update merge request by specifying a new title of the merge request | | 1.80.4 | [link](https://docs.gitlab.com/cli/mr/update/) |
| `glab mr create -b <target_branch_name> -t <title> --remove-source-branch` | create merge request for a currently checked out branch on the target branch with a flag specifying to delete remote source branch after the merge | | 1.80.4 | [link](https://docs.gitlab.com/cli/mr/create/) |
| `glab mr list` | list all merge requests | | 1.80.4 | [link](https://docs.gitlab.com/cli/mr/list/) | |
| `glab mr rebase` | rebase remote source branch against its target branch | local branch is not changing by this command | 1.80.4 | [link](https://docs.gitlab.com/cli/mr/rebase/) |

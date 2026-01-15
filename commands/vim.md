| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `/<search_term>` | find the term going forward | type `n` for the next find and `b` for the previous one | 5.1.4 | |
| `:%d` | delete all lines | | 5.1.4 | |
| `:%s/<serach_term_1>/<search_term_2>/gc` | find the first search term and replace it with the second one with confirmation before every replacement | | 5.1.4 | |
| `:%y` | copy all lines | | 5.1.4 | |
| `:<<` | de-indent line by the number of spaces specified by the `shiftwidh` property | `shiftwidh` defines number of spaces for indentation | 5.1.4 | |
| `:<line_number>` | jump to the specified line | | 5.1.4 | |
| `:<range>!<ext_filter> <filter_args>` | filter a range of lines through an external program | without the `<range>`, only the current line is filtered, range will automaticaly become `'<,'>` for visual selection | 5.1.4 | |
| `:>>` | indent line by the number of spaces specified by the `shiftwidh` property | `shiftwidh` defines number of spaces for indentation | 5.1.4 | |
| `:file` | show the filename | | 5.1.4 | |
| `:g/^$/d` | delete all blank lines in the working file | | 5.1.4 | |
| `:set list` | display whitespace characters | spaces are shown as ` `, tabs as `^I`, and the end-of-line as a `$`| 5.1.4 | |
| `:set mouse=` | disable mouse | | 5.1.4 | |
| `:set mouse=a` | enable mouse | | 5.1.4 | |
| `:set nolist` | hide whitespace characters | | 5.1.4 | |
| `:set nonumber` | hide line numbers | alias command is `:set nonu` | 5.1.4 | |
| `:set number` | display line numbers | alias command is `:set nu` | 5.1.4 | |
| `:term` | open terminal window | 5.1.4 | |
| `?<search_term>` | find the term going backward | type `n` for the next find and `b` for the previous one | 5.1.4 | |

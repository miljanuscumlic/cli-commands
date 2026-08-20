| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `npm ci` | clean install of dependencies | its primary use is with continuous integration, test platforms... | 9.9.4 | [link](https://docs.npmjs.com/cli/v9/commands/npm-ci) |
| `npm config get cache` | show path to the npm cache directory | | 9.2.0 | [link](https://docs.npmjs.com/cli/v9/commands/npm-config) |
| `npm i` | install package and its dependencies | `package.json` must be present in a directory; command respects contetnt of `package-lock.js` file | 9.2.0 | [link](https://docs.npmjs.com/cli/v9/commands/npm-install) |
| `npm i --offline` | npm offline mode using only dependencies present in local cache | command fails if requeseted package is not available in cache | 9.2.0 | |
| `npm i -D <package_name>` | install package used in development | it won't be intsalled in production environment | 9.2.0 | [link](https://docs.npmjs.com/cli/v9/commands/npm-install) | 
| `npm i -g <package_name>` | install package globally in `/usr/local` directory so it can be run in terminal | 9.2.0 | [link](https://docs.npmjs.com/cli/v9/commands/npm-install) |
| `npm rm  <package_name>` | remove given package | | 9.2.0 | [link](https://docs.npmjs.com/cli/v9/commands/npm-uninstall) |

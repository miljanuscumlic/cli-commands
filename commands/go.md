| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `go get -u ./...` | update all dependencies to their latest minor version | | 1.24.2 | |
| `go mod tidy` | clean up unnecessary dependencies | | 1.24.2 | [link](https://go.dev/doc/modules/managing-dependencies#synchronizing) |
| `go mod verify` | check that dependencies have not been modified after their download | | 1.24.2 | [link](https://go.dev/ref/mod#go-mod-verify) |
| `go get <package_name>@latest` | update dependency to the latest major version | | 1.24.2 | [link](https://pkg.go.dev/cmd/go#hdr-Add_dependencies_to_current_module_and_install_them) |
| `go list -m -u all \| awk '{print $1}' \| xargs -n 1 go get -u` | update all dependencies to their latest minor or major version | | 1.24.2 | |

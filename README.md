# go
Uber repo for examples and courses on the Go programming language


---

# Setting up Go Environment
- Go: Download and install Go from the official website: https://go.dev/
  - Check version: `go version`
- VS Code: Install the Go Extension from the Go Team at Google
  
---

# Individual Example Setup
- Create module: outputs the file `go.mod` 
go mod init example.com/first-app

- Run application
go run app.go

- Build application: outputs the binary file `first-app`
go build -o first-app app.go

- Run the built application
./first-app

- Debug application in VS Code: see `.vscode/launch.json` configuration below:
```json
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Launch file",
            "type": "go",
            "request": "launch",
            "mode": "debug",
            "program": "${file}"
        },
        {
            "name": "Launch Package",
            "type": "go",
            "request": "launch",
            "mode": "auto",
            "program": "${workspaceFolder}"
        }
    ]
}
```


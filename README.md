# -Develop-from-anywhere-with-Visual-Studio-Code

https://www.youtube.com/live/dggcqfGe1xs?feature=share 

Architecture

UI Process                Extension Host Process         Worker Processes 
Desktop or Web         Desktop, Web or Remote       

Download Visual Studio Code Insiders 
https://code.visualstudio.com/docs/?dv=win&build=insiders 

Control Shift P
Developer Open Process Explorer 

A Remote World 

WSL: Full linux distro on Windows

Dev Containers: Reproducible dev containers

Remote SSH: Remote machines

Github Codespaces: Instant dev environment 


Scenario 1
I need to develop my app on another machine ( Remote SSH ) 

Visual Studio Code - Insiders 

https://github.com/devcontainers/devcontainers.github.io 

Settings 
Profile 
Create Profile 
Remote 

EXTENSIONS 
Remote Development 

><
Connect Current Window to Host 
Add New SSH Host
Rodrigomvs123

c:\Users\Rodrigomvs123> uname
Windows 
c:\Users\Rodrigomvs123> git clone https://github.com/devcontainers/devcontainers.github.io.git
https://github.com/devcontainers/devcontainers.github.io 
c:\Users\Rodrigomvs123> 

EXTENSIONS 
LOCAL INSTALLED 
Remote Development 

SSH: RODRIGOMVS123 - Insiders
Github Copilot 
[                     ]

Rodrigomvs123
What language is my project written in ?

Github Copilot
Your project appears to be Jekill for building a website, which is a static site generator written in Ruby. Therefore, your project is likely written in Ruby along with HTML, CSS and possibly JavaScript for the website itself.

Scenario 2 
I need to develop an app in a toolchain I do not have ( Dev Containers )

Visual Studio Code - Insiders 
Explorer 
Develop from anywhere with visual studio code 
devcontainers.github.io
.devcontainer
devcontainer.json

devcontainer.json
// For format details, see https://aka.ms/devcontainer.json. For config options, see the
// README at: https://github.com/devcontainers/templates/tree/main/src/jekyll
{
	"name": "Jekyll",
	// Or use a Dockerfile or Docker Compose file. More info: https://containers.dev/guide/dockerfile
	"image": "mcr.microsoft.com/devcontainers/jekyll:1-bullseye",

	// Features to add to the dev container. More info: https://containers.dev/features.
	"features": {
		"ghcr.io/devcontainers/features/node:1": {
		  "version": "latest"
		}
	},

	// Use 'forwardPorts' to make a list of ports inside the container available locally.
	"forwardPorts": [
		// Jekyll server
		4000,
		// Live reload server
		35729
	]

	// Uncomment the next line to run commands after the container is created.
	// "postCreateCommand": "jekyll --version"

	// Configure tool-specific properties.
	// "customizations": {},

	// Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
	// "remoteUser": "root"
}

Visual Studio Code
SSH Rodrigomvs123
Select an option to open a Remote Window
Add Dev Container Configuration Files
Select a container configuration template
jek
Jekill devcontainers
Debian OS version (use bookworm, or bullseye on local arm64/Apple Silicon):
bullseye (default) 
Select additional features to install

Visual Studio Code
SSH Rodrigomvs123
Select an option to open a Remote Window
Reopen in Container

Dev Container jekyll@ssh://Rodrigomvs123

Visual Studio Code
SSH Rodrigomvs123
Select an option to open a Remote Window
Tasks: Run Tasks 
Serve
Terminal
Open in Browser
localhost:4000
Development Containers   Overview    ….
 
                                                    Development Containers 
What are Development Containers ?

https://code.visualstudio.com/docs/devcontainers/containers 

Scenario 3
I need a really really big machine ( Github Codespaces )


EXTENSIONS 
LOCAL INSTALLED 
Remote Development 
Github Codespaces

Visual Studio Code
Remote Explorer Dev Containers ( Github Codespaces )
Remote Explorer
Dev Containers
devcontainers.github.io
Github Codespaces
Create Codespace 
devcontainers.github.io
devcontainers.github.i0[Codespaces] - Visual Studio Code - Insiders
 
Visual Studio Code - Insiders 
Explorer 
Develop from anywhere with visual studio code 
devcontainers.github.io
.devcontainer
devcontainer.json

devcontainer.json
// For format details, see https://aka.ms/devcontainer.json. For config options, see the
// README at: https://github.com/devcontainers/templates/tree/main/src/jekyll
{
	"name": "Jekyll",
	// Or use a Dockerfile or Docker Compose file. More info: https://containers.dev/guide/dockerfile
	"image": "mcr.microsoft.com/devcontainers/jekyll:1-bullseye",

	// Features to add to the dev container. More info: https://containers.dev/features.
	"features": {
		"ghcr.io/devcontainers/features/node:1": {
		  "version": "latest"
		},
                        "ghcr.io/devcontainers/features/node:1": {
		  "version": "latest"
		}
	},

	// Use 'forwardPorts' to make a list of ports inside the container available locally.
	"forwardPorts": [
		// Jekyll server
		4000,
		// Live reload server
		35729
	]

	// Uncomment the next line to run commands after the container is created.
	// "postCreateCommand": "jekyll --version"

	// Configure tool-specific properties.
	// "customizations": {},

	// Uncomment to connect as root instead. More info: https://aka.ms/dev-containers-non-root.
	// "remoteUser": "root"
}

Visual Studio Code
Source Control
Add Ruby feature 
  
Commit ( Save and Commit )
Sync Changes 

Visual Studio Code
Github 
PULL REQUESTS
…
ISSUES
…

Visual Studio Code
Github 
Create
Merge Changes From 
Remote …
Branch …

INTO
Remote …
Branch …

Title 
Add Ruby feature 
Description 
More Ruby ?
Create as a Draft 
Create 

Pull Request #261
Add Ruby feature #261
Draft
Rodrigomvs123 wants to merge changes into devcontainers:gh-pages from devcontainers:Rodrigomvs123
Reviews                                               Assignees

Labels                                                   Milestone

Rodrigomvs123 commented seconds ago Peding
More Ruby ?

Scenario 4
I want to review some code without disrupting my local environment 

Github Repository 
devcontainers / devcontainers.github.io
Pull Requests
Add Ruby feature
Pull Request #261
Add Ruby feature #261
Draft
Rodrigomvs123 wants to merge changes into devcontainers:gh-pages from 
Conversations            Comments 20           Checks 1              Files Changed 2
devcontainers:Rodrigomvs123
Reviews                                               Assignees

Labels                                                   Milestone

Rodrigomvs123 commented seconds ago Peding
More Ruby ?

Visual Studio Code ( Browser ) 
Repository path + vscode.dev/
https://vscode.dev/github/devcontainers/devcontainers.github.io

Visual Studio Code - Insiders 
Explorer 
Develop from anywhere with visual studio code 
devcontainers.github.io
.devcontainer
spec.github-issues 

Scenario 5
I want to develop from the beach ! ( Remote Tunnels ) 

Tunneling and an enhanced code CLI
Access  remote machines vie secure tunnels, no SSH or HTTPS required
Build tunneling directly into code CLI vs VS Code UI
Remote-Tunnels extension
Prompt 
C:\Users\Matheus> code-insiders tunnel - -help
C:\Users\Matheus> code-insiders tunnel
https://insiders.vscode.dev/tunnel/…

Docs: https://aka.ms/vscode-remote 
Remote Extensions: https://aka.ms/vscode-remote-extensions 
VS Code for the Web: https://vscode.dev
Issue or feature request: https://aka.ms/vscode-remote/issues 



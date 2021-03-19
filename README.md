# vcat
Version Control Centered around FTP

# About
Getting tired of git's s****y commands, after I'm done with gasp I will begin focus on creating a new VC with more thought out commands, however I don't want the hassle of trying to implement security so I will stick to FTP and whoever is in control of the server can think about the security stuff, an example of a command will look like this:

```
vcat --branch a b
...
vcat --commit --server --branch *
```
The only concept of locality will be stored in .vcat, all commits will default to local (hence the --server option), vcat will assume a project structure like this:
```
.vcat/*.lua
tree/[BRANCH]/*
tree/[BRANCH]/.vcat/commits.lua
tree/[BRANCH]/.vcat/commits/[TIMESTAMP]/*
```

Naturally the .vcat folder will contain settings relavent to the project, using lua means that security can be customised, using FTP means I don't have to provide a server like github for the software, I will naturally create a test ground but I won't share that, instead you need to get your own server.

As for the name vcat, I simply thought that up on the spot after thinking what short name can I use with VC, for now the only thing I can think of for the acronym to stand for is Version Control Advanced Tool, I don't intend to change the Version Control part but I'd like to remove the Advanced part in favour of something less arrogant, open to suggestions there

Git commands

## Alias
#### Delete all merged branches
```
bclean = "!f() { git checkout ${1-master} && git branch --merged ${1-master} | grep -v " ${1-master}$" | xargs git branch -d; }; f"
```

#### View git tree
```
lola = log --oneline --decorate --all --graph
```
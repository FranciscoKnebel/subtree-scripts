# subtree-scripts

# Criado usando git subtree
https://developer.atlassian.com/blog/2015/05/the-power-of-git-subtree/

###### $HOME/.gitconfig

```
[alias]
# "subtree add"
  sba = "!f() { ./path/to/scripts/add }; f"
# "subtree remove"
  sbr = "!f() { ./path/to/scripts/remove }; f"
# "subtree update"
  sbu = "!f() { ./path/to/scripts/update }; f"
# "subtree update all"
  sbua = "!f() { ./path/to/scripts/updateAll }; f"
```

##### ADD repository folder
```
git sba <repository uri> <destination folder>
```

##### REMOVE repository folder
```
git sbr <destination folder>
```

##### UPDATE repository folder
```
git sbu <repository uri> <destination folder>
```

##### UPDATE ALL repository folder

```
git sbua
```

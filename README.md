# subtree-scripts
Scripts to add, remove and update subtrees inside a repository.

##### Created using git subtree
https://developer.atlassian.com/blog/2015/05/the-power-of-git-subtree/

## Getting Started
Clone the repository to your local machine and update your `.gitconfig` file with the configuration provided on the next step.

### Prerequisites
- Git.

### Installing
After you clone the repository, copy the full path to the `scripts` directory.

###### $HOME/.gitconfig

Add this configuration to your .gitconfig file.
`path/to/scripts` should be set accordingly.

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

After you configure `.gitconfig`, you can use the scripts as defined on the usage section.

### Usage

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

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/franciscoknebel/subtree-scripts/tags).

## Authors

* **Francisco Knebel** - *Initial work* - [Francisco Knebel](https://github.com/FranciscoKnebel)

See also the list of [contributors](https://github.com/FranciscoKnebel/subtree-scripts/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

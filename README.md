# Publish
A Simple publish and deploy script written in ruby (Fire breathing dragon included)

# Usage
`publish [OPTIONS]`

- `--tag <tag>` Will push the given tag. Specifying `v1.2.1`.  It will create a tag with `v1.2.1`
- `--berks` Will run `berks upload` then `berks update` after all the git operations
- `--kitchen` Will run `kitchen test` before all the git operations
- `--banch <branch>` will push to the specified branch
- `--remote <remote>` will push to the specified remote

# Recommendations

If you want to make things easy put this in your `.bash_profile`

```
alias publish="publish --berks --branch development --version "
```


type `reload` then use publish as so to publish a new release

```
publish <version>
```
# Publish
A Simple publish and deploy script written in ruby (Fire breathing dragon included)

# Usage
`publish <version> [OPTIONS]`

- `<version>` is required and should be something like `1.2.1`.  It will create a tag with `v1.2.1`
- `--berks` Will run `berks upload` and `berks update` after all the git operations
- `--kitchen` Will run `kitchen test` before all the git operations
- `--banch <branch>` will push to the specified branch
- `--remote <remote>` will push to the specified remote

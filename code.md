# Semantic Versioning

- Semver is short
- Homepage: [https://semver.org](https://semver.org)
- Use three numbers in versioning

## Automatically generating CHANGELOGs

- See: [Conventional Changelog](https://github.com/conventional-changelog/conventional-changelog)
- After instructions, we will use [Standard Version](https://github.com/conventional-changelog/standard-version)
- Install cli via NPM:

```bash
npm install -g standard-version
standard-version --version
```

## How it works

1. when you land commits on your master branch, select the Squash and Merge option.
2. add a title and body that follows the Conventional Commits Specification.
3. when you're ready to release:
4. ```bash git checkout master; git pull origin master```
5. run `standard-version`
6. git push --follow-tags origin master && npm publish (or, docker push, gem push, etc.)

## Commands

```bash
standard-version --help
standard-version --release-as 0.2.0
standard-version --first-release
```

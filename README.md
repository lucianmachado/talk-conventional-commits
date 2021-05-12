
## [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.4/)

The Conventional Commits specification is a lightweight convention on top of commit messages.
It provides an easy set of rules for creating an explicit commit history;
which makes it easier to write automated tools on top of.
This convention dovetails with [SemVer](http://semver.org),
by describing the features, fixes, and breaking changes made in commit messages.

The commit message should be structured as follows:

---

```
<type>[optional scope]: <description>

[optional body]

[optional footer]
```
---

<br />
The commit contains the following structural elements, to communicate intent to the
consumers of your library:

1. **fix:** a commit of the _type_ `fix` patches a bug in your codebase (this correlates with [`PATCH`](http://semver.org/#summary) in semantic versioning).
1. **feat:** a commit of the _type_ `feat` introduces a new feature to the codebase (this correlates with [`MINOR`](http://semver.org/#summary) in semantic versioning).
1. **BREAKING CHANGE:** a commit that has the text `BREAKING CHANGE:` at the beginning of its optional body or footer section introduces a breaking API change (correlating with [`MAJOR`](http://semver.org/#summary) in semantic versioning).
A BREAKING CHANGE can be part of commits of any _type_.
1. Others: commit _types_ other than `fix:` and `feat:` are allowed, for example [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/tree/master/%40commitlint/config-conventional) (based on the [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)) recommends `chore:`, `docs:`, `style:`, `refactor:`, `perf:`, `test:`, and others.

We also recommend `improvement` for commits that improve a current implementation without adding a new feature or fixing a bug.
Notice these types are not mandated by the conventional commits specification, and have no implicit effect in semantic versioning (unless they include a BREAKING CHANGE).
<br />
A scope may be provided to a commit's type, to provide additional contextual information and is contained within parenthesis, e.g., `feat(parser): add ability to parse arrays`.

## Examples

### Commit message with description and breaking change in body
```
feat: allow provided config object to extend other configs

BREAKING CHANGE: `extends` key in config file is now used for extending other config files
```

### Commit message with optional `!` to draw attention to breaking change
```
chore!: drop Node 6 from testing matrix

BREAKING CHANGE: dropping Node 6 which hits end of life in April
```

### Commit message with no body
```
docs: correct spelling of CHANGELOG
```

### Commit message with scope
```
feat(lang): add polish language
```

### Commit message for a fix using an (optional) issue number.
```
fix: correct minor typos in code

see the issue for details on the typos fixed

closes issue #12
```


https://www.conventionalcommits.org/en/v1.0.0-beta.4/


## Why ?
Automatically generating CHANGELOGs

Automatically determining a semantic version bump (based on the types of commits landed)

Communicating the nature of changes to teammates, the public, and other stakeholders

Triggering build and publish processes

Making it easier for people to contribute to your projects, by allowing them to explore a more structured commit history

## [Semantic-release](https://github.com/semantic-release/semantic-release)
semantic-release automates the whole package release workflow including: determining the next version number, generating the release notes and publishing the package.

This removes the immediate connection between human emotions and version numbers, strictly following the Semantic Versioning specification.


```
https://github.com/semantic-release/semantic-release/blob/master/docs/extending/plugins-list.md
https://github.com/semantic-release/commit-analyzer
https://github.com/semantic-release/git
https://github.com/semantic-release/changelog
https://github.com/semantic-release/release-notes-generator
https://github.com/semantic-release/exec
https://github.com/semantic-release/npm
```



### Angular Commit Convention

https://github.com/angular/angular/blob/master/CONTRIBUTING.md#-commit-message-format



## Projects
https://github.com/nodejs/node/commits/master
https://github.com/angular/angular/commits/master

## Release Notes
https://nodejs.org/en/blog/release/v16.1.0/
https://github.com/semantic-release/semantic-release
https://docs.npmjs.com/about-semantic-versioning


## Semantic Versioning
https://docs.npmjs.com/about-semantic-versioning


## Useful Tools



https://github.com/conventional-changelog/conventional-changelog
https://github.com/aevea/commitsar
https://github.com/conventional-changelog/standard-version
https://github.com/talos-systems/conform



https://dev.azure.com/lucianmachado/talkcc/_workitems/edit/1/

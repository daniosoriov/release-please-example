# Press Release Example

This is a working example repository of [Press Release](https://github.com/googleapis/release-please).

## Setup

Follow the steps to create a [PR Action workflow](https://github.com/google-github-actions/release-please-action).

Be sure to create a 
[Personal Access Token (PAT)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) from GitHub and assign the value of the token to 
the `MY_RELEASE_PLEASE_TOKEN` secret in the repository.

The PAT needs to have writing permissions on the following Repository permissions:
- `Contents`
- `Pull Requests`

## Usage

### File changing, committing and pushing

Make file changes to any files to make a test.

Then, commit and push them to the `master` branch. 
Be sure to follow the [Conventional Commits messages](https://www.conventionalcommits.org/) format.

#### Commit message example

```bash
git commit -m "docs: changing the README.md to include a new section"
```

### Creating a release

The GitHub action will automatically create a pull request with the release notes.

**Merge and squash** the pull request to create a release.

The file `CHANGELOG.md` will be updated with the release notes.

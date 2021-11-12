# Checkity.io upload action

This action uploads code coverage reports to [checkity.io](https://checkity.io), see it in action in our [upload-example](https://github.com/checkity/upload-example) repository.

## Usage

See [action.yml](action.yml).

```yaml
- uses: checkity/upload@v1
  with:
    # Comma separated list of coverage files to upload, supports globs. 
    file-pattern: '**/jacoco.xml,**/lcov.info'

    # The GitHub token used to validate repository access when uploading coverage reports.
    repo-token: ${{ secrets.GITHUB_TOKEN }}
```

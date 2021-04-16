# Checkity.io upload action

This action uploads code coverage reports to [checkity.io](https://checkity.io), see it in action in our [upload-example](https://github.com/checkity/upload-example) repository.

## Usage

```yaml
- uses: checkity/upload@v1
  with:
    # Comma separated list of coverage report paths, supports globs. 
    # Default: **/jacoco.xml
    coverage-report-paths: '**/jacoco.xml'

    # The GitHub token used to validate repository access when uploading coverage reports.
    repo-token: ${{ secrets.GITHUB_TOKEN }}
```

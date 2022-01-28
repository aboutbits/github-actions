# GitHub Web Actions

A collection of GitHub actions for web projects.

## Example Playbook

```yaml
  - name: Build code
    uses: aboutbits/github-web-actions/node-build@v1
    with:
      node-version: ${{ env.NODE_VERSION }}
```

## Versioning

In order to have a verioning in place and working, create leightweight tags that point to the appropriate minor release versions.

Creating a new minor release:

```bash
git tag v1
git push --tags
```

Replacing an already existing minor release:

```bash
git tag -d v1
git push origin :refs/tags/v1
git tag v1
git push --tags
```

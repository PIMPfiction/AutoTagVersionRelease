# AutoTagVersionRelease

_This GitHub action creates tag in every push and creates release from this tag as latest.

## Features

- Creates Tag in every push
- Releases new version labeled as "latest" with tag
- Uses phish108/autotag-action@1.1.51 for auto tagging
- Uses official checkout and script actions for release

## Usage

Just copy and paste whole action.yml or use below usage directly.

```yaml
jobs:
  release:
    runs-on: ubuntu-latest
    steps:
      - uses: PIMPfiction/AutoTagVersionRelease@v1
      with:
        github-token: ${{ secrets.GITHUB_TOKEN}}
```

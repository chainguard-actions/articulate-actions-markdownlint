# markdownlint action

This action lints your Markdown files with [markdownlint-cli](https://github.com/igorshubovych/markdownlint-cli).

## Usage

Including the action without any defaults will find a local markdownlint config
file (`.markdownlint.{yaml,yml,json}`) or use our included default and scan all
files with the `md` or `markdown` extension.

```yaml
- uses: articulate/actions-markdownlint@v1
```

You can set the config file, the files it scans, or files/directories to ignore.

```yaml
- uses: articulate/actions-markdownlint@v1
  with:
    config: markdownlint-config.json
    files: 'docs/**/*.md'
    ignore: node_modules
```

## Privacy

This Action contacts Chainguard's licensing server to verify authorization. Connection metadata (IP address, GitHub repository identifier, timestamp, and any metadata encoded in the auth token) is transmitted to Chainguard, Inc. even if authorization is denied in accordance with our [Privacy Notice](https://www.chainguard.dev/legal/privacy-notice)

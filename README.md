# homebrew-tap

Homebrew formulae for [anyq](https://github.com/troll-warlord/anyq) — a unified
jq-syntax query tool for JSON, YAML, and TOML.

## Install

```bash
brew install troll-warlord/tap/anyq
```

Or tap first, then install:

```bash
brew tap troll-warlord/tap
brew install anyq
```

## Upgrade

```bash
brew upgrade anyq
```

## Uninstall

```bash
brew uninstall anyq
brew untap troll-warlord/tap  # optional
```

## Usage

```bash
# Query JSON
anyq '.name' file.json

# Query YAML
anyq '.services.web.image' docker-compose.yml

# Query TOML
anyq '.package.version' Cargo.toml

# Diff two files (any format)
anyq diff old.json new.yaml

# Validate against a JSON Schema
anyq validate --schema schema.json data.yaml
```

Full documentation: https://github.com/troll-warlord/anyq

## Reporting Issues

Please open issues on the main repository:
https://github.com/troll-warlord/anyq/issues

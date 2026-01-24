# Homebrew Tap for ali-nuke

This is the official Homebrew tap for [ali-nuke](https://github.com/arafato/alicloud-nuke), a command-line tool to delete all resources from an Alibaba Cloud account.

## Installation

```bash
brew tap arafato/tap
brew install ali-nuke
```

Or install directly:

```bash
brew install arafato/tap/ali-nuke
```

## Upgrade

```bash
brew upgrade ali-nuke
```

## Usage

```bash
# Dry run (default) - shows what would be deleted
ali-nuke nuke \
  --config config.yaml \
  --access-key-id <YOUR_ACCESS_KEY_ID> \
  --access-key-secret <YOUR_ACCESS_KEY_SECRET>

# Actually delete resources
ali-nuke nuke \
  --config config.yaml \
  --access-key-id <YOUR_ACCESS_KEY_ID> \
  --access-key-secret <YOUR_ACCESS_KEY_SECRET> \
  --no-dry-run
```

## Documentation

For full documentation, see the [ali-nuke repository](https://github.com/arafato/alicloud-nuke).

## License

MIT

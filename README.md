# Homebrew Tap

This is the official Homebrew tap for cloud infrastructure tools by [@arafato](https://github.com/arafato).

## Available Formulas

| Formula | Description |
|---------|-------------|
| [cf-nuke](https://github.com/arafato/cf-nuke) | Delete all resources from a Cloudflare account |
| [ali-nuke](https://github.com/arafato/alicloud-nuke) | Delete all resources from an Alibaba Cloud account |

## Installation

First, add the tap:

```bash
brew tap arafato/tap
```

Then install the tools you need:

```bash
brew install cf-nuke
brew install ali-nuke
```

Or install directly without adding the tap first:

```bash
brew install arafato/tap/cf-nuke
brew install arafato/tap/ali-nuke
```

## Upgrade

```bash
brew upgrade cf-nuke
brew upgrade ali-nuke
```

## cf-nuke Usage

```bash
# Dry run (default) - shows what would be deleted
cf-nuke nuke \
  --config config.yaml \
  --api-token <YOUR_CLOUDFLARE_API_TOKEN>

# Actually delete resources
cf-nuke nuke \
  --config config.yaml \
  --api-token <YOUR_CLOUDFLARE_API_TOKEN> \
  --no-dry-run
```

For full documentation, see the [cf-nuke repository](https://github.com/arafato/cf-nuke).

## ali-nuke Usage

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

For full documentation, see the [ali-nuke repository](https://github.com/arafato/alicloud-nuke).

## License

MIT

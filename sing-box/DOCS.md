# sing-box add-on documentation

## Configuration

`config_url` is required and must point to a remote sing-box `config.json`.

Example:

```yaml
config_url: https://example.com/config.json
```

On start, the add-on downloads the configuration to a temporary file, runs `sing-box check`, then atomically replaces the active config.

## Runtime

The add-on runs with host networking and `NET_ADMIN` so sing-box can create TUN interfaces.

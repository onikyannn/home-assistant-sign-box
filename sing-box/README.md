# sing-box

sing-box proxy service for Home Assistant.

The add-on downloads a remote `config.json`, validates it with `sing-box check`, and starts sing-box with persistent state under `/data/state`.

## Configuration

```yaml
config_url: https://example.com/config.json
```

## Notes

- The URL should point to a valid sing-box JSON configuration.
- The add-on uses host networking and requires `/dev/net/tun`.
- The full config URL is not printed to logs.

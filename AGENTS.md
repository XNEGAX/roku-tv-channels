<!-- roku-tv-channels — Channel list data repo consumed by the canal-chileno Roku app -->

Single `channels.json` consumed at runtime via:
```
https://raw.githubusercontent.com/XNEGAX/roku-tv-channels/main/channels.json
```

Format: JSON array of `{"name": "...", "url": "..."}` entries (HLS .m3u8 streams), grouped by region (Chile, International, AR, CO, PE, ES, MX) with blank-line separators.

Edit, commit, push — the Roku app picks up changes on next cache refresh (1h TTL). No build, test, or deploy step.

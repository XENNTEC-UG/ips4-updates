# IPS4 Update Check

Static JSON endpoint for IPS4 app update checks, served via GitHub Pages.

Each `{app}.json` file returns the latest version info in IPS4's expected format:

```json
{
    "version": "1.0.0",
    "longversion": 10000,
    "released": 1700000000,
    "updateurl": "https://github.com/XENNTEC-UG/ips4-{app}/releases"
}
```

These files are automatically updated by GitHub Actions when a new release is published in any app repo.

**Endpoint:** `https://xenntec-ug.github.io/ips4-updates/{app}.json`

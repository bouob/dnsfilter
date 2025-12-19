# Line Ads DNS Block List

**Last Updated**: 2025-12-19
**Source**: [Gslin's Blog - Blocking Line Ads on Desktop and Laptop](https://blog.gslin.org/archives/2025/12/16/12795/)

---

## Overview

This list blocks advertising and tracking domains used by Line on desktop and laptop applications. Blocking these domains can significantly reduce ads displayed in the Line application.

---

## Blocked Domains

### Advertising Domains

| Domain | Purpose |
|--------|---------|
| `a.line.me` | Main advertising server |
| `ad.line-scdn.net` | Ad content delivery |

### News/Today Service

| Domain | Purpose |
|--------|---------|
| `api.today.line.me` | Today tab API (includes ads) |
| `today.line.me` | Today news service |
| `today-obs.line-scdn.net` | Today service CDN |

### Tracking & Analytics

| Domain | Purpose |
|--------|---------|
| `crs-event.line.me` | Event tracking |
| `linecrs.line-scdn.net` | CRS (Customer Relationship Service) tracking |
| `jp-col-tcp.nelo.linecorp.com` | NELO logging service |

### LEGY (Line Edge Gateway)

| Domain | Purpose |
|--------|---------|
| `legy.line-apps.com` | Edge gateway for ad delivery |
| `legy.line-apps.com.akadns.net` | Akamai CDN for LEGY |
| `legy-jp-addr-ds.line-apps.com` | Japan LEGY address service |

### VOOM (Timeline/Social Feed)

| Domain | Purpose |
|--------|---------|
| `voom-assets.line-scdn.net` | VOOM assets (includes ads) |
| `voom-obs.line-scdn.net` | VOOM observation/tracking |

### Other Services

| Domain | Purpose |
|--------|---------|
| `sch.line.me` | Search/scheduling service |
| `uts-front.line-apps.com` | UTS frontend service |
| `w.line.me` | Web widget service |

---

## Usage

### AdGuard Home

Add this URL to your blocklist:
```
https://raw.githubusercontent.com/bouob/dnsfilter/main/list/line.txt
```

### Pi-hole

Convert the list format or add domains individually.

### Hosts file

Add the following to your hosts file:
```
0.0.0.0 a.line.me
0.0.0.0 ad.line-scdn.net
0.0.0.0 api.today.line.me
0.0.0.0 crs-event.line.me
0.0.0.0 jp-col-tcp.nelo.linecorp.com
0.0.0.0 legy.line-apps.com
0.0.0.0 legy.line-apps.com.akadns.net
0.0.0.0 legy-jp-addr-ds.line-apps.com
0.0.0.0 linecrs.line-scdn.net
0.0.0.0 sch.line.me
0.0.0.0 today.line.me
0.0.0.0 today-obs.line-scdn.net
0.0.0.0 uts-front.line-apps.com
0.0.0.0 voom-assets.line-scdn.net
0.0.0.0 voom-obs.line-scdn.net
0.0.0.0 w.line.me
```

---

## Notes

1. **Desktop/Laptop Focus**: This list is specifically designed for blocking Line ads on desktop and laptop applications, not mobile devices.

2. **Core Functionality**: Blocking these domains should not affect Line's core messaging functionality.

3. **Today Tab**: Blocking `today.line.me` and related domains will disable the Today/News tab in Line.

4. **VOOM**: Blocking VOOM domains will reduce social feed ads but may affect timeline functionality.

---

## References

- [Gslin's Blog - Blocking Line Ads](https://blog.gslin.org/archives/2025/12/16/12795/)

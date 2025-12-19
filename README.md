# DNS Filter Lists

A collection of DNS blocklists for AdGuard Home, Pi-hole, and other DNS-based ad blockers.

## Available Lists

| List | Description | Domains | Link |
|------|-------------|---------|------|
| **Xiaohongshu** | Block Xiaohongshu (RedNote) tracking and services | 20+ | [xiaohongshu.txt](list/xiaohongshu.txt) |
| **Line Ads** | Block Line advertising and tracking | 18 | [line.txt](list/line.txt) |

## Usage

### AdGuard Home

1. Go to **Filters** > **DNS blocklists**
2. Click **Add blocklist** > **Add a custom list**
3. Enter the raw URL of the list:

```
https://raw.githubusercontent.com/bouob/dnsfilter/main/list/xiaohongshu.txt
https://raw.githubusercontent.com/bouob/dnsfilter/main/list/line.txt
```

### Pi-hole

1. Go to **Adlists** in the Pi-hole admin panel
2. Add the raw URL of the list
3. Run `pihole -g` to update gravity

### Hosts File

See the documentation in `docs/` folder for hosts file format.

## Documentation

Detailed domain documentation is available in the `docs/` folder:

- [Xiaohongshu Domains](docs/xiaohongshu-domains.md) - Comprehensive list of Xiaohongshu domains and their purposes
- [Line Domains](docs/line-domains.md) - Line advertising and tracking domains

## List Format

All lists use the AdGuard Home filter syntax:

```
||domain.com^
```

This format blocks the domain and all its subdomains.

## Contributing

Contributions are welcome! If you know of additional domains that should be blocked, please open an issue or submit a pull request.

## Disclaimer

These blocklists are provided for privacy and ad-blocking purposes. Use at your own discretion. Blocking certain domains may affect the functionality of applications.

## License

This project is licensed under the [AGPL-3.0 License](LICENSE).

## References

### Xiaohongshu
- [SRLabs - Xiaohongshu Security Analysis](https://srlabs.de/blog/xiaohongshu-little-red-book-reads-you)
- [EFF - Crimson Memo: Analyzing Privacy Impact of Xiaohongshu](https://www.eff.org/deeplinks/2025/02/crimson-memo-analyzing-privacy-impact-xiaohongshu-aka-red-note)

### Line
- [Gslin's Blog - Blocking Line Ads on Desktop and Laptop](https://blog.gslin.org/archives/2025/12/16/12795/)
- [MrPeel's Blog - Using AdGuard to Remove Line Ads](https://mrpeelblog.com/posts/line-adblock/)

# Note taking

SHIVERS should maintain a daily log of activities. SHIVERS use a mixture of shared Slack Canvases (WYSIWYG Markdown editor) and individual solutions. 

## Obsidian for individual note takiong

[Obsidian - Sharpen your thinking](https://obsidian.md/) is a free (but not open-source) Markdown editor that works across desktops/laptops and mobile phones. Christian has used open-source alternative [Logseq](https://logseq.com) for 1 year in 2023 on Windows and macOS, then switched to Obsidian since 2025 after this tool became free to use including for commercial use.

### Setup iSH on iPhones for synchronizing Obsidian vaults via git

Requires an iPhone.

Install [iSH](https://ish.app) ([GitHub repository](https://github.com/ish-app/ish)) under iOS so that you can sync via ssh your Obsidian notes Vault, that is versioned in a git repository that is local to your phone and that is local to your desktop/laptop.

#### Git optimization on iPhones

Once you open iSH, set:
```
git config --global pack.threads "1"
```
otherwise git commands inside iSH can take forever, found out via [Git Commands Stuck Forever · Issue #1640 · ish-app/ish](https://github.com/ish-app/ish/issues/1640).

#### (Optional) Setup literal IP addresses in git remotes

Not yet solved.

You might have to use literal IP addresses in git remotes instead of `.local` hostnames, but that looks fixable:
- [Unable to SSH into Raspberry Pi using Hostname.local in iSH App · Issue #2238 · ish-app/ish](https://github.com/ish-app/ish/issues/2238)
- [mDNS - Alpine Linux](https://wiki.alpinelinux.org/wiki/MDNS)

# Installation
Add this to `/etc/portage/repos.conf/tthanh`.

```
[sk-overlay]
location   = /usr/local/overlay/tt-overlay
sync-type  = git
sync-uri   = https://github.com/tthanh/overlay.git
auto-sync  = yes
```

`/usr/local/overlay` doesn't exist by default so create it if needed.

```
[ ! -d /usr/local/overlay ] && mkdir -p /usr/local/overlay
```

Finally you can update portage.

```
emerge --sync
```

# harbour

xbps binary repository for Devoid — a curated subset of the
[voidlab overlay](https://github.com/mendescotta/voidlab).

Contains only the dinit boot stack and the packages needed to build and
install Devoid. No runit-intercompat packages, no full DE stacks.

## Adding the repository

```
# echo 'repository=https://github.com/mendescotta/harbour/releases/download/repo' \
    > /etc/xbps.d/20-harbour.conf
# xbps-install -S
```

## Package set

Defined in [`tools/packages`](tools/packages). The CI runs daily, syncing
approved packages from the voidlab release and publishing them here.

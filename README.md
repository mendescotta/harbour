# voidlab-packages

xbps binary repository for voidlab — a curated subset of the
[voidlab-testing overlay](https://github.com/mendescotta/voidlab-testing).

Contains only the dinit boot stack and the packages needed to build and
install voidlab. No runit-intercompat packages, no full DE stacks.

## Adding the repository

```
# echo 'repository=https://github.com/mendescotta/voidlab-packages/releases/download/repo' \
    > /etc/xbps.d/20-voidlab-packages.conf
# xbps-install -S
```

## Package set

Defined in [`tools/packages`](tools/packages). The CI runs daily, syncing
approved packages from the voidlab-testing release and publishing them here.

# OrangeFox Recovery Project for the Samsung Galaxy J7 2017

### How to build ###

```bash
# Create dirs
$ mkdir ofox ; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone my local repo
$ git clone https://gitlab.com/Device7870/manifest/android_manifest_samsung_j7y17lte.git -b orangefox .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ mv device/samsung/j7y17lte/build_ofox.sh .
$ . build_ofox.sh j7y17lte
```
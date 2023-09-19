### ApolloOS ###

### Sync ###
```bash
        repo init -u https://github.com/ApolloOS/manifest.git -b 13
        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###
```bash
	. build/envsetup.sh
        brunch device
```


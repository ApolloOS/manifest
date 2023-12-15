<img src="banner.png">
<p align="center">

## ApolloOS

## Initializing Repository

**Repo initialization**

    repo init -u https://github.com/ApolloOS/manifest.git -b 14-qpr1 --git-lfs

**Sync repo**

    repo sync -c --force-sync --no-tags --no-clone-bundle -j10 --optimized-fetch --prune

## Options

	APOLLO_BUILD_VARIANT - (vanilla, gapps, foss, microg) - We currently use this to specify what type of extra apps and services to include in the build. 
***Note: Default APOLLO_BUILD_VARIANT is VANILLA.***

## Building

     . build/envsetup.sh
     apolloify options deviceCodename

**Examples:**

- **To build with gapps**
```
     apolloify -g deviceCodename
```

- **To build with FOSS**
```
     apolloify -f deviceCodename
```

- **To build with gapps and deviceclean**
```
     apolloify -g -d deviceCodename
```

**This method is also backwards compatible with the legacy apolloify command also**
```
     apolloify deviceCodename
```

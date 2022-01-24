# Pixel Experience X #
# Born with the idea to maintain device with the original functions, without adding on device anything that does not work properly. #
# Is also born with the idea to add the best things a rom can offer without distorting the base "PIXEL" #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/PixelExperienceX/manifest -b twelve

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ make bacon -jX
```

### Submitting Patches ###

Patches are always welcome! Please submit your patches by pull request.

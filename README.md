# ODH-Nightlies disconnected install helper

This repository contains the updated list of additional images needed to install ODH-Nightlies in a disconnected environment using oc-mirror for the current releases supported by RHODS.

The list of images and versions are updated automatically by a GitHub action.

## How to use it

You can copy the list directly from the repository or use the script to get the list of images for the version you want to install.

### 1. Copy the list of images from the repository:

Copy the list from the file of the version you want to install and paste it in the additionalImages section of the ImageSetConfiguration file you are using to mirror the images. In the file there is also an example of ImageSetConfiguration.

### 2. Run the script locally:
#### Requirements:
- bash 4.0 or higher
- jq latest
- oc latest
- yq latest
- skopeo latest

#### Usage:

Example:
```bash
./odh-nightlies-disconnected-helper.sh
```

To get help about the script
```bash
./odh-nightlies-disconnected-helper.sh -h
```

After running the script, the list of images with an example will be saved in a file by default called odh-nightlies.md.
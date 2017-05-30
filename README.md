# Show XMP crs Crop information

**Bash script to display CRS Crop information stored in XMP Meta tags. Uses XMP sidecar file if used on RAW files.**

Requires Phil Harvey's [exiftool](http://www.sno.phy.queensu.ca/~phil/exiftool/) which is installable via Homebrew.


## Usage

```bash
$ show-crop image1 [ images ...]
```

## Example

```bash
$ show-crop image-nocrop.tif "image-cropped.tiff" "test-cropped.NEF"

# First image
Warning: No CRS crop data available for 'image-nocrop.tif'.

# Second image image
image-cropped.tiff
HasCrop: True
CropTop: 0.113804
CropLeft: 0.129985
CropBottom: 0.621707
CropRight: 0.868538
CropAngle: 0
CropWidth:
CropHeight:
CropUnits:

# Third image
Warning: Image 'test-cropped.NEF' itself has no CRS crop data, use XMP sidecar instead: test-cropped.xmp
test-cropped.xmp
HasCrop: True
CropTop: 0.02378
CropLeft: 0.075063
CropBottom: 0.87985
CropRight: 0.710592
CropAngle: 0
CropWidth:
CropHeight:
CropUnits:
```

## Development

```bash
$ git clone https://github.com/tomkyle/show-crop.git
```




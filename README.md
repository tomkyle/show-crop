# Show XMP crs Crop information

Bash script to display CRS Crop information stored in XMP Meta tags.  
Requires Phil Harvey's [exiftool](http://www.sno.phy.queensu.ca/~phil/exiftool/) which is installable via Homebrew.


## Usage

```bash
$ show-crop image1 [ images ...]
```

Outputs: 

```
$ show-crop image1.tif "image1 cropped.tiff"

Warning: Image 'image1.tif' has no CRS Crop Data.

image1 cropped.tiff
HasCrop: True
CropTop: 0.113804
CropLeft: 0.129985
CropBottom: 0.621707
CropRight: 0.868538
CropAngle: 0
CropWidth:
CropHeight:
CropUnits:
```

## Development

```bash
$ git clone https://github.com/tomkyle/show-crop.git
```




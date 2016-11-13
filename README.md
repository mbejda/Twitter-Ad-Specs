![](https://github.com/mbejda/Twitter-Ad-Specs/blob/master/TwitterAds.png)

# Twitter Ad Specifications
**source :** [https://business.twitter.com/en/help/campaign-setup/advertiser-card-specifications.html](https://business.twitter.com/en/help/campaign-setup/advertiser-card-specifications.html)
## Table
| Type  | Dimensions | Format | Aspect Ratio |
|---|---|------------|--------|--------------|
| Website Card | 800px by 320px | JPG or PNG |
| Lead Generation Card | 800px by 200px | JPG or PNG  |
| Business APP Card | 144px by 144px| JPG or PNG |
| Image APP Card | 800px by 320px | JPG or PNG |
| Video Thumbnail | 640px by 360px | JPG or PNG | 16:9 |
| Single Image Tweets (mobile) | 600px by 335px <br> Recommended : 1200px by 675px  | PNG, JPEG, or GIF | 16:9 |
| Single Image Tweets (desktop) | Recommended  1200px by 1200px | PNG, JPEG, or GIF | _Any aspect between 2:1 and 1:1 is acceptable. Cropped to 1:1_ |
| Summary Card With Large Image | min  280px by 150px | PNG, JPEG, or GIF | 2:1 |
| Conversational Ads |  800px by 320px |  PNG, JPEG, non-animated GIFs| 5:2 |

<hr>
## JSON 
For those who only read JSON formats : 
```json
{
    "Website Card": {
        "width": 800,
        "height": 320,
        "format": ["JPG", "PNG"]

    },
    "Lead Generation Card": {
        "width": 800,
        "height": 200,
        "format": ["JPG", "PNG"]
    },
    "Business APP Card": {
        "width": 144,
        "height": 144,
        "format": ["JPG", "PNG"]
    },
    "Image APP Card": {
        "width": 800,
        "height": 320,
        "format": ["JPG", "PNG"]
    },
    "Video Thumbnail": {
        "width": 640,
        "height": 360,
        "aspectRatio": [16, 9],
        "format": ["JPG", "PNG"]
    },
    "Single Image Tweet": {
        "mobile": {
            "width": 1200,
            "height": 675,
            "aspectRatio": [16, 9],
            "format": ["JPG", "PNG", "GIF"]
        },
        "desktop": {
            "width": 1200,
            "height": 1200,
            "aspectRatio": [1, 1],
            "format": ["JPG", "PNG", "GIF"]
        },
    },
    "Summary Card With Large Image": {
        "min": {
            "width": 280,
            "height": 150
        },
        "aspectRatio": [2, 1],
        "format": ["JPG", "PNG", "GIF"]
    },
    "Conversational Ads": {
        "width": 800,
        "height": 320,
        "aspectRatio": [5, 2],
        "format": ["JPG", "PNG", "GIF"]
    }

}
```

<hr>



## Twitter Cards


### Website Card
- Tweet copy: 116 characters are available (24 characters are used for images).

- Website title length: 70 characters. Please note — depending on device and app settings this description may truncate. Although not guaranteed, limiting the description to 50 characters should ensure that truncation won’t occur across most devices.

- Image size: 800 x 320 pixels (max 3mb)

- File types: PNG and JPEG are recommended. We do not accept BMP or TIFF files.

### Lead Generation Card

- Tweet copy: 116 characters are available (24 characters are used for images).

- Short description: 50 characters (only appears on desktop).

- Post submit message: Text after lead is submitted, 100 characters.

- Image size: 800 x 200 pixels (max 3mb).

- File types: PNG and JPEG are recommended. We do not accept BMP or TIFF files.

- Call-to-action options: Custom, 20 character limit.


### Business APP Card

- Tweet copy: 116 characters are available (24 characters are used for images).

- Custom icon image size: 144 x 144 pixels.

- File types: PNG and JPEG are recommended. We do not accept BMP or TIFF files.

- Title/price: Pulled from app store.

- Call-to-action options: Install (default if app is not installed), Open (default if app is installed), Play, Shop, Book, Connect, and Order.


### Image APP Card

- Tweet copy: 116 characters are available (24 characters are used for images).

- Image size: 800 x 320 pixels (max 3mb).

- File types: PNG and JPEG are recommended. We do not accept BMP or TIFF files.

- Title/price: Pulled from app store.

- Call to action options: Install (default if app is not installed), Open (default if app is installed), Play, Shop, Book, Connect, and Order.


### Video App Card

- Tweet copy: 116 characters are available (24 characters are used for images).

- See “Video” section above for detailed video creative specifications.


## Videos

### Promoted Videos

- Tweet copy: 140 characters.

- Title (under video): 70 characters.

- Description (under video): 200 characters.

- File type: MP4 or MOV.

- File size: Under 1GB strongly recommended for optimal performance.

- Max time: 2 minutes and 20 seconds (10 minute access available for select accounts, reach out to your Twitter rep for more information).

- Video codec recommendation: H264, Baseline, Main, or High profile with a 4:2:0 color space.

- Frame rate recommendation: 29.97FPS or 30FPS. Higher is acceptable. If the available video has a lower frame rate don’t try to “upsample” it.

- Video bitrate recommendation: 6,000 - 10,000k (recommended 6,000k) for 1080p. 5,000k - 8,000k (recommended 5,000k) for 720p).

- Audio codec recommendation: AAC LC (low complexity).


### Video  Thumbnail
- Supported file types: PNG or JPEG.

- Recommended aspect ratio: 16:9

- Minimum size: 640 pixels by 360 pixels.

- Max size: 5mb


## Single Image Tweets & Gifs

Note: When using the same image across desktop and mobile, we recommend sticking to the mobile specs — which will work across both. Selecting desktop specifications may result in cropping on mobile.
 

###  Mobile
- Tweet copy: 140 characters are available when composing Tweets using www.twitter.com or our native applications. Only 116 characters are available for Tweets composed using ads.twitter.com, as 24 characters are used for the image when composing Tweets in that workflow.

- Image width/height: Minimum 600 X 335 pixels, although larger images (for example 1200 X 675) will be better optimized for when users click to expand images.

- Aspect ratio: 16:9.

Image file size: Max 15mb on twitter.com and 3mb on ads.twitter.com.
File types: PNG, JPEG, or GIF are recommended. We do not accept BMP or TIFF files.
 

### Desktop
- Tweet copy: 140 characters are available when composing Tweets using www.twitter.com or our native applications. Only 116 characters are available for Tweets composed using ads.twitter.com, as 24 characters are used for the image when composing Tweets in that workflow.

- Image width/height: We recommend a minimum width of 600 pixels, although larger images (for example 1200 pixel images) will be better optimized for when users click to expand images. Any height is acceptable, although if the height exceeds the width, we will crop to 1:1 (see aspect ratio details).

- Aspect ratio: Any aspect between 2:1 and 1:1 is acceptable. For example, 1200 X 600 (2:1), 1200 X 800 (3:2) or 1200 X 1200 (1:1). After 1:1 aspect ratio (for example, 1200 X 1400) we’ll crop to a 1:1 aspect ratio.

- Image file size: Max 15mb on twitter.com & 3mb on ads.twitter.com.
File types: PNG, JPEG, or GIF are recommended. We do not accept BMP or TIFF files.


## Summary Card With Large Image
 
- Tweet copy: 116 characters are available (24 characters are used for images).

- Title: Truncated at 70 characters.

- Description: Truncated at 200 characters.

- Image size: 280 x 150 pixels (minimum), 1mb max.

- File types: PNG, JPEG, or GIF are recommended. We do not accept BMP or TIFF files.

- Aspect ratio: 2:1


## Conversational Ads
- Tweet copy: 116 characters are available (24 characters are used for the Conversational Card).

- Hashtag: 21 characters.

- Pre-populated user Tweet: 116 characters.
Headline: 23 characters.

- Thank you text: 23 characters.

- Thank you URL (optional): 23 characters.

- Video (if used): Same specifications mentioned in the “Promoted video” section.

- Image Specs (if used): File size: 3 MB, Aspect ratio: 5:2, Image width / height: 800 X 320PX, File formats: JPEG, PNG, non-animated GIFs.


<hr>



*Send me a tweet!*<br>
[@notmilobejda](https://twitter.com/notmilobejda) <br>
[Blog](https://mbejda.com)


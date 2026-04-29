---
description: These settings apply to a specific graphic overlay. You can include multiple overlays in your job.
layout: schema
name: InsertableImage
properties_list:
- description: ''
  name: Duration
  type: object
- description: ''
  name: FadeIn
  type: object
- description: ''
  name: FadeOut
  type: object
- description: ''
  name: Height
  type: object
- description: ''
  name: ImageInserterInput
  type: object
- description: ''
  name: ImageX
  type: object
- description: ''
  name: ImageY
  type: object
- description: ''
  name: Layer
  type: object
- description: ''
  name: Opacity
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Width
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-insertable-image-schema.json
slug: mediaconvert-api-insertable-image
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-insertable-image-schema.json\",\n  \"title\": \"InsertableImage\",\n  \"description\": \"These settings apply to a specific graphic overlay. You can include multiple overlays in your job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"duration\"\n          },\n          \"description\": \"Specify the time, in milliseconds, for the image to remain on the output video. This duration includes fade-in time but not fade-out time.\"\n        }\n      ]\n    },\n    \"FadeIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"fadeIn\"\n          },\n          \"description\": \"Specify the length of time, in milliseconds, between the Start time that you specify for the image insertion and the time that the image appears at full opacity. Full opacity is the level that you specify for the opacity setting. If you don't specify a value for Fade-in, the image will appear abruptly at the overlay start time.\"\n        }\n      ]\n    },\n    \"FadeOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fadeOut\"\n          },\n          \"description\": \"Specify the length of time, in milliseconds, between the end of the time that you have specified for the image overlay Duration and when the overlaid image has faded to total transparency. If you don't specify a value for Fade-out, the image will disappear abruptly at the end of the\
  \ inserted image duration.\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"Specify the height of the inserted image in pixels. If you specify a value that's larger than the video resolution height, the service will crop your overlaid image to fit. To use the native height of the image, keep this setting blank.\"\n        }\n      ]\n    },\n    \"ImageInserterInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin14PatternS3BmpBMPPngPNGTgaTGAHttpsBmpBMPPngPNGTgaTGA\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageInserterInput\"\n          },\n          \"description\": \"Specify the HTTP, HTTPS, or Amazon S3 location of the image that you want to overlay on the video. Use a PNG or TGA file.\"\
  \n        }\n      ]\n    },\n    \"ImageX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageX\"\n          },\n          \"description\": \"Specify the distance, in pixels, between the inserted image and the left edge of the video frame. Required for any image overlay that you specify.\"\n        }\n      ]\n    },\n    \"ImageY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageY\"\n          },\n          \"description\": \"Specify the distance, in pixels, between the overlaid image and the top edge of the video frame. Required for any image overlay that you specify.\"\n        }\n      ]\n    },\n    \"Layer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max99\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"layer\"\n          },\n          \"description\": \"Specify how overlapping inserted images appear. Images with higher values for Layer appear on top of images with lower values for Layer.\"\n        }\n      ]\n    },\n    \"Opacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"opacity\"\n          },\n          \"description\": \"Use Opacity (Opacity) to specify how much of the underlying video shows through the inserted image. 0 is transparent and 100 is fully opaque. Default is 50.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern01D20305D205D\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"description\": \"Specify the timecode of the frame that you\
  \ want the overlay to first appear on. This must be in timecode (HH:MM:SS:FF or HH:MM:SS;FF) format. Remember to take into account your timecode source settings.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"Specify the width of the inserted image in pixels. If you specify a value that's larger than the video resolution width, the service will crop your overlaid image to fit. To use the native width of the image, keep this setting blank.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-insertable-image-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InsertableImage
---

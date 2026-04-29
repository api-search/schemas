---
description: Settings for the action to activate a static image.
layout: schema
name: StaticImageActivateScheduleActionSettings
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
  name: Image
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
  name: Width
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-static-image-activate-schedule-action-settings-schema.json
slug: medialive-api-static-image-activate-schedule-action-settings
source_filename: medialive-api-static-image-activate-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-static-image-activate-schedule-action-settings-schema.json\",\n  \"title\": \"StaticImageActivateScheduleActionSettings\",\n  \"description\": \"Settings for the action to activate a static image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"duration\"\n          },\n          \"description\": \"The duration in milliseconds for the image to remain on the video. If omitted or set to 0 the duration is unlimited and the image will remain until it is explicitly deactivated.\"\n        }\n      ]\n    },\n    \"FadeIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"fadeIn\"\n          },\n          \"description\": \"The time in milliseconds for the image to fade in. The fade-in starts at the start time of the overlay. Default is 0 (no fade-in).\"\n        }\n      ]\n    },\n    \"FadeOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fadeOut\"\n          },\n          \"description\": \"Applies only if a duration is specified. The time in milliseconds for the image to fade out. The fade-out starts when the duration time is hit, so it effectively extends the duration. Default is 0 (no fade-out).\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"The height\
  \ of the image when inserted into the video, in pixels. The overlay will be scaled up or down to the specified height. Leave blank to use the native height of the overlay.\"\n        }\n      ]\n    },\n    \"Image\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"image\"\n          },\n          \"description\": \"The location and filename of the image file to overlay on the video. The file must be a 32-bit BMP, PNG, or TGA file, and must not be larger (in pixels) than the input video.\"\n        }\n      ]\n    },\n    \"ImageX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageX\"\n          },\n          \"description\": \"Placement of the left edge of the overlay relative to the left edge of the video frame, in pixels. 0 (the default) is the left edge\
  \ of the frame. If the placement causes the overlay to extend beyond the right edge of the underlying video, then the overlay is cropped on the right.\"\n        }\n      ]\n    },\n    \"ImageY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageY\"\n          },\n          \"description\": \"Placement of the top edge of the overlay relative to the top edge of the video frame, in pixels. 0 (the default) is the top edge of the frame. If the placement causes the overlay to extend beyond the bottom edge of the underlying video, then the overlay is cropped on the bottom.\"\n        }\n      ]\n    },\n    \"Layer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"layer\"\n          },\n          \"description\": \"The number of the layer, 0 to 7. There are\
  \ 8 layers that can be overlaid on the video, each layer with a different image. The layers are in Z order, which means that overlays with higher values of layer are inserted on top of overlays with lower values of layer. Default is 0.\"\n        }\n      ]\n    },\n    \"Opacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"opacity\"\n          },\n          \"description\": \"Opacity of image where 0 is transparent and 100 is fully opaque. Default is 100.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"The width of the image when inserted into the video, in pixels. The overlay will be scaled up or down to the specified width. Leave blank to use the native\
  \ width of the overlay.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-static-image-activate-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StaticImageActivateScheduleActionSettings
---

---
description: Use these settings to specify static color calibration metadata, as defined by SMPTE ST 2086. These values don't affect the pixel values that are encoded in the video stream. They are intended to help the downstream video player display content in a way that reflects the intentions of the the content creator.
layout: schema
name: Hdr10Metadata
properties_list:
- description: ''
  name: BluePrimaryX
  type: object
- description: ''
  name: BluePrimaryY
  type: object
- description: ''
  name: GreenPrimaryX
  type: object
- description: ''
  name: GreenPrimaryY
  type: object
- description: ''
  name: MaxContentLightLevel
  type: object
- description: ''
  name: MaxFrameAverageLightLevel
  type: object
- description: ''
  name: MaxLuminance
  type: object
- description: ''
  name: MinLuminance
  type: object
- description: ''
  name: RedPrimaryX
  type: object
- description: ''
  name: RedPrimaryY
  type: object
- description: ''
  name: WhitePointX
  type: object
- description: ''
  name: WhitePointY
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hdr10-metadata-schema.json
slug: mediaconvert-api-hdr10-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hdr10-metadata-schema.json\",\n  \"title\": \"Hdr10Metadata\",\n  \"description\": \"Use these settings to specify static color calibration metadata, as defined by SMPTE ST 2086. These values don't affect the pixel values that are encoded in the video stream. They are intended to help the downstream video player display content in a way that reflects the intentions of the the content creator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BluePrimaryX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bluePrimaryX\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools.\
  \ Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n    },\n    \"BluePrimaryY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bluePrimaryY\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n    },\n    \"GreenPrimaryX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"greenPrimaryX\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader,\
  \ using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n    },\n    \"GreenPrimaryY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"greenPrimaryY\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n    },\n    \"MaxContentLightLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxContentLightLevel\"\n          },\n          \"description\": \"Maximum light level\
  \ among all samples in the coded video sequence, in units of candelas per square meter. This setting doesn't have a default value; you must specify a value that is suitable for the content.\"\n        }\n      ]\n    },\n    \"MaxFrameAverageLightLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxFrameAverageLightLevel\"\n          },\n          \"description\": \"Maximum average light level of any frame in the coded video sequence, in units of candelas per square meter. This setting doesn't have a default value; you must specify a value that is suitable for the content.\"\n        }\n      ]\n    },\n    \"MaxLuminance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxLuminance\"\n          },\n          \"description\": \"Nominal\
  \ maximum mastering display luminance in units of of 0.0001 candelas per square meter.\"\n        }\n      ]\n    },\n    \"MinLuminance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minLuminance\"\n          },\n          \"description\": \"Nominal minimum mastering display luminance in units of of 0.0001 candelas per square meter\"\n        }\n      ]\n    },\n    \"RedPrimaryX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"redPrimaryX\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n\
  \    },\n    \"RedPrimaryY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"redPrimaryY\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n    },\n    \"WhitePointX\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitePointX\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\
  \n        }\n      ]\n    },\n    \"WhitePointY\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max50000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitePointY\"\n          },\n          \"description\": \"HDR Master Display Information must be provided by a color grader, using color grading tools. Range is 0 to 50,000, each increment represents 0.00002 in CIE1931 color coordinate. Note that this setting is not for color correction.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hdr10-metadata-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Hdr10Metadata
---

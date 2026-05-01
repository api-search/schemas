---
description: Use automated ABR to have MediaConvert set up the renditions in your ABR package for you automatically, based on characteristics of your input video. This feature optimizes video quality while minimizing the overall size of your ABR package.
layout: schema
name: AutomatedAbrSettings
properties_list:
- description: ''
  name: MaxAbrBitrate
  type: object
- description: ''
  name: MaxRenditions
  type: object
- description: ''
  name: MinAbrBitrate
  type: object
- description: ''
  name: Rules
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-automated-abr-settings-schema.json
slug: mediaconvert-api-automated-abr-settings
source_filename: mediaconvert-api-automated-abr-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-automated-abr-settings-schema.json\",\n  \"title\": \"AutomatedAbrSettings\",\n  \"description\": \"Use automated ABR to have MediaConvert set up the renditions in your ABR package for you automatically, based on characteristics of your input video. This feature optimizes video quality while minimizing the overall size of your ABR package.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxAbrBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxAbrBitrate\"\n          },\n          \"description\": \"Optional. The maximum target bit rate used in your automated ABR stack. Use this value to set an upper limit on the bandwidth consumed by\
  \ the highest-quality rendition. This is the rendition that is delivered to viewers with the fastest internet connections. If you don't specify a value, MediaConvert uses 8,000,000 (8 mb/s) by default.\"\n        }\n      ]\n    },\n    \"MaxRenditions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin3Max15\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxRenditions\"\n          },\n          \"description\": \"Optional. The maximum number of renditions that MediaConvert will create in your automated ABR stack. The number of renditions is determined automatically, based on analysis of each job, but will never exceed this limit. When you set this to Auto in the console, which is equivalent to excluding it from your JSON job specification, MediaConvert defaults to a limit of 15.\"\n        }\n      ]\n    },\n    \"MinAbrBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max100000000\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"minAbrBitrate\"\n          },\n          \"description\": \"Optional. The minimum target bitrate used in your automated ABR stack. Use this value to set a lower limit on the bitrate of video delivered to viewers with slow internet connections. If you don't specify a value, MediaConvert uses 600,000 (600 kb/s) by default.\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAutomatedAbrRule\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rules\"\n          },\n          \"description\": \"Optional. Use Automated ABR rules to specify restrictions for the rendition sizes MediaConvert will create in your ABR stack. You can use these rules if your ABR workflow has specific rendition size requirements, but you still want MediaConvert to optimize for video quality and overall file size.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-automated-abr-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AutomatedAbrSettings
---

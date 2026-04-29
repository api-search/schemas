---
description: Placeholder documentation for VideoBlackFailoverSettings
layout: schema
name: VideoBlackFailoverSettings
properties_list:
- description: ''
  name: BlackDetectThreshold
  type: object
- description: ''
  name: VideoBlackThresholdMsec
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-black-failover-settings-schema.json
slug: medialive-api-video-black-failover-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-black-failover-settings-schema.json\",\n  \"title\": \"VideoBlackFailoverSettings\",\n  \"description\": \"Placeholder documentation for VideoBlackFailoverSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlackDetectThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blackDetectThreshold\"\n          },\n          \"description\": \"A value used in calculating the threshold below which MediaLive considers a pixel to be 'black'. For the input to be considered black, every pixel in a frame must be below this threshold. The threshold is calculated as a percentage (expressed as a decimal) of white. Therefore .1 means 10% white (or 90% black). Note\
  \ how the formula works for any color depth. For example, if you set this field to 0.1 in 10-bit color depth: (1023*0.1=102.3), which means a pixel value of 102 or less is 'black'. If you set this field to .1 in an 8-bit color depth: (255*0.1=25.5), which means a pixel value of 25 or less is 'black'. The range is 0.0 to 1.0, with any number of decimal places.\"\n        }\n      ]\n    },\n    \"VideoBlackThresholdMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoBlackThresholdMsec\"\n          },\n          \"description\": \"The amount of time (in milliseconds) that the active input must be black before automatic input failover occurs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-black-failover-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoBlackFailoverSettings
---

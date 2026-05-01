---
description: Settings for quality-defined variable bitrate encoding with the H.264 codec. Use these settings only when you set QVBR for Rate control mode (RateControlMode).
layout: schema
name: H264QvbrSettings
properties_list:
- description: ''
  name: MaxAverageBitrate
  type: object
- description: ''
  name: QvbrQualityLevel
  type: object
- description: ''
  name: QvbrQualityLevelFineTune
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h264-qvbr-settings-schema.json
slug: mediaconvert-api-h264-qvbr-settings
source_filename: mediaconvert-api-h264-qvbr-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-qvbr-settings-schema.json\",\n  \"title\": \"H264QvbrSettings\",\n  \"description\": \"Settings for quality-defined variable bitrate encoding with the H.264 codec. Use these settings only when you set QVBR for Rate control mode (RateControlMode).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxAverageBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max1152000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxAverageBitrate\"\n          },\n          \"description\": \"Use this setting only when Rate control mode is QVBR and Quality tuning level is Multi-pass HQ. For Max average bitrate values suited to the complexity of your input video, the service limits the average bitrate of the video\
  \ part of this output to the value that you choose. That is, the total size of the video element is less than or equal to the value you set multiplied by the number of seconds of encoded output.\"\n        }\n      ]\n    },\n    \"QvbrQualityLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qvbrQualityLevel\"\n          },\n          \"description\": \"Use this setting only when you set Rate control mode (RateControlMode) to QVBR. Specify the target quality level for this output. MediaConvert determines the right number of bits to use for each part of the video to maintain the video quality that you specify. When you keep the default value, AUTO, MediaConvert picks a quality level for you, based on characteristics of your input video. If you prefer to specify a quality level, specify a number from 1 through 10. Use higher numbers for greater quality. Level 10\
  \ results in nearly lossless compression. The quality level for most broadcast-quality transcodes is between 6 and 9. Optionally, to specify a value between whole numbers, also provide a value for the setting qvbrQualityLevelFineTune. For example, if you want your QVBR quality level to be 7.33, set qvbrQualityLevel to 7 and set qvbrQualityLevelFineTune to .33.\"\n        }\n      ]\n    },\n    \"QvbrQualityLevelFineTune\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"qvbrQualityLevelFineTune\"\n          },\n          \"description\": \"Optional. Specify a value here to set the QVBR quality to a level that is between whole numbers. For example, if you want your QVBR quality level to be 7.33, set qvbrQualityLevel to 7 and set qvbrQualityLevelFineTune to .33. MediaConvert rounds your QVBR quality level to the nearest third of a whole number. For example, if you set qvbrQualityLevel\
  \ to 7 and you set qvbrQualityLevelFineTune to .25, your actual QVBR quality level is 7.33.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-qvbr-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: H264QvbrSettings
---

---
description: Specify the XAVC profile settings for MXF outputs when you set your MXF profile to XAVC.
layout: schema
name: MxfXavcProfileSettings
properties_list:
- description: ''
  name: DurationMode
  type: object
- description: ''
  name: MaxAncDataSize
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mxf-xavc-profile-settings-schema.json
slug: mediaconvert-api-mxf-xavc-profile-settings
source_filename: mediaconvert-api-mxf-xavc-profile-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mxf-xavc-profile-settings-schema.json\",\n  \"title\": \"MxfXavcProfileSettings\",\n  \"description\": \"Specify the XAVC profile settings for MXF outputs when you set your MXF profile to XAVC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DurationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MxfXavcDurationMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"durationMode\"\n          },\n          \"description\": \"To create an output that complies with the XAVC file format guidelines for interoperability, keep the default value, Drop frames for compliance (DROP_FRAMES_FOR_COMPLIANCE). To include all frames from your input in this output, keep the default setting, Allow any duration (ALLOW_ANY_DURATION). The\
  \ number of frames that MediaConvert excludes when you set this to Drop frames for compliance depends on the output frame rate and duration.\"\n        }\n      ]\n    },\n    \"MaxAncDataSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxAncDataSize\"\n          },\n          \"description\": \"Specify a value for this setting only for outputs that you set up with one of these two XAVC profiles: XAVC HD Intra CBG (XAVC_HD_INTRA_CBG) or XAVC 4K Intra CBG (XAVC_4K_INTRA_CBG). Specify the amount of space in each frame that the service reserves for ancillary data, such as teletext captions. The default value for this setting is 1492 bytes per frame. This should be sufficient to prevent overflow unless you have multiple pages of teletext captions data. If you have a large amount of teletext data, specify a larger number.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mxf-xavc-profile-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MxfXavcProfileSettings
---

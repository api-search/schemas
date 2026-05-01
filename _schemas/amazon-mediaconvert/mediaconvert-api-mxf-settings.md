---
description: These settings relate to your MXF output container.
layout: schema
name: MxfSettings
properties_list:
- description: ''
  name: AfdSignaling
  type: object
- description: ''
  name: Profile
  type: object
- description: ''
  name: XavcProfileSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mxf-settings-schema.json
slug: mediaconvert-api-mxf-settings
source_filename: mediaconvert-api-mxf-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mxf-settings-schema.json\",\n  \"title\": \"MxfSettings\",\n  \"description\": \"These settings relate to your MXF output container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AfdSignaling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MxfAfdSignaling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"afdSignaling\"\n          },\n          \"description\": \"Optional. When you have AFD signaling set up in your output video stream, use this setting to choose whether to also include it in the MXF wrapper. Choose Don't copy (NO_COPY) to exclude AFD signaling from the MXF wrapper. Choose Copy from video stream (COPY_FROM_VIDEO) to copy the AFD values from the video stream for this output to the MXF wrapper. Regardless\
  \ of which option you choose, the AFD values remain in the video stream. Related settings: To set up your output to include or exclude AFD values, see AfdSignaling, under VideoDescription. On the console, find AFD signaling under the output's video encoding settings.\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MxfProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"Specify the MXF profile, also called shim, for this output. When you choose Auto, MediaConvert chooses a profile based on the video codec and resolution. For a list of codecs supported with each MXF profile, see https://docs.aws.amazon.com/mediaconvert/latest/ug/codecs-supported-with-each-mxf-profile.html. For more information about the automatic selection behavior, see https://docs.aws.amazon.com/mediaconvert/latest/ug/default-automatic-selection-of-mxf-profiles.html.\"\
  \n        }\n      ]\n    },\n    \"XavcProfileSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MxfXavcProfileSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavcProfileSettings\"\n          },\n          \"description\": \"Specify the XAVC profile settings for MXF outputs when you set your MXF profile to XAVC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mxf-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MxfSettings
---

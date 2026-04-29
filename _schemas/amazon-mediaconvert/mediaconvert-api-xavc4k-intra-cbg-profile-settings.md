---
description: Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K_INTRA_CBG.
layout: schema
name: Xavc4kIntraCbgProfileSettings
properties_list:
- description: ''
  name: XavcClass
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc4k-intra-cbg-profile-settings-schema.json
slug: mediaconvert-api-xavc4k-intra-cbg-profile-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc4k-intra-cbg-profile-settings-schema.json\",\n  \"title\": \"Xavc4kIntraCbgProfileSettings\",\n  \"description\": \"Required when you set (Profile) under (VideoDescription)>(CodecSettings)>(XavcSettings) to the value XAVC_4K_INTRA_CBG.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"XavcClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Xavc4kIntraCbgProfileClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavcClass\"\n          },\n          \"description\": \"Specify the XAVC Intra 4k (CBG) Class to set the bitrate of your output. Outputs of the same class have similar image quality over the operating points that are valid for that class.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc4k-intra-cbg-profile-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Xavc4kIntraCbgProfileSettings
---

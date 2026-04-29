---
description: Specifies DRM settings for DASH outputs.
layout: schema
name: DashIsoEncryptionSettings
properties_list:
- description: ''
  name: PlaybackDeviceCompatibility
  type: object
- description: ''
  name: SpekeKeyProvider
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-iso-encryption-settings-schema.json
slug: mediaconvert-api-dash-iso-encryption-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-encryption-settings-schema.json\",\n  \"title\": \"DashIsoEncryptionSettings\",\n  \"description\": \"Specifies DRM settings for DASH outputs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PlaybackDeviceCompatibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashIsoPlaybackDeviceCompatibility\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"playbackDeviceCompatibility\"\n          },\n          \"description\": \"This setting can improve the compatibility of your output with video players on obsolete devices. It applies only to DASH H.264 outputs with DRM encryption. Choose Unencrypted SEI (UNENCRYPTED_SEI) only to correct problems with playback on older devices. Otherwise, keep the default setting CENC\
  \ v1 (CENC_V1). If you choose Unencrypted SEI, for that output, the service will exclude the access unit delimiter and will leave the SEI NAL units unencrypted.\"\n        }\n      ]\n    },\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          },\n          \"description\": \"If your output group type is HLS, DASH, or Microsoft Smooth, use these settings when doing DRM encryption with a SPEKE-compliant key provider. If your output group type is CMAF, use the SpekeKeyProviderCmaf settings instead.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-encryption-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashIsoEncryptionSettings
---

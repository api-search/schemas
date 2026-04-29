---
description: If you are using DRM, set DRM System (MsSmoothEncryptionSettings) to specify the value SpekeKeyProvider.
layout: schema
name: MsSmoothEncryptionSettings
properties_list:
- description: ''
  name: SpekeKeyProvider
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ms-smooth-encryption-settings-schema.json
slug: mediaconvert-api-ms-smooth-encryption-settings
source_filename: mediaconvert-api-ms-smooth-encryption-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ms-smooth-encryption-settings-schema.json\",\n  \"title\": \"MsSmoothEncryptionSettings\",\n  \"description\": \"If you are using DRM, set DRM System (MsSmoothEncryptionSettings) to specify the value SpekeKeyProvider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SpekeKeyProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpekeKeyProvider\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spekeKeyProvider\"\n          },\n          \"description\": \"If your output group type is HLS, DASH, or Microsoft Smooth, use these settings when doing DRM encryption with a SPEKE-compliant key provider. If your output group type is CMAF, use the SpekeKeyProviderCmaf settings instead.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ms-smooth-encryption-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MsSmoothEncryptionSettings
---

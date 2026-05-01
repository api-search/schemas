---
description: Output Group settings, including type
layout: schema
name: OutputGroupSettings
properties_list:
- description: ''
  name: CmafGroupSettings
  type: object
- description: ''
  name: DashIsoGroupSettings
  type: object
- description: ''
  name: FileGroupSettings
  type: object
- description: ''
  name: HlsGroupSettings
  type: object
- description: ''
  name: MsSmoothGroupSettings
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-group-settings-schema.json
slug: mediaconvert-api-output-group-settings
source_filename: mediaconvert-api-output-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-settings-schema.json\",\n  \"title\": \"OutputGroupSettings\",\n  \"description\": \"Output Group settings, including type\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CmafGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cmafGroupSettings\"\n          },\n          \"description\": \"Settings related to your CMAF output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to CMAF_GROUP_SETTINGS.\"\n        }\n      ]\n    },\n\
  \    \"DashIsoGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashIsoGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dashIsoGroupSettings\"\n          },\n          \"description\": \"Settings related to your DASH output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to DASH_ISO_GROUP_SETTINGS.\"\n        }\n      ]\n    },\n    \"FileGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileGroupSettings\"\n          },\n          \"description\": \"Settings related to your File output group. MediaConvert uses this group of settings to generate a single standalone file,\
  \ rather than a streaming package. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to FILE_GROUP_SETTINGS.\"\n        }\n      ]\n    },\n    \"HlsGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsGroupSettings\"\n          },\n          \"description\": \"Settings related to your HLS output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to HLS_GROUP_SETTINGS.\"\n        }\n      ]\n    },\n    \"MsSmoothGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothGroupSettings\"\n        },\n        {\n     \
  \     \"xml\": {\n            \"name\": \"msSmoothGroupSettings\"\n          },\n          \"description\": \"Settings related to your Microsoft Smooth Streaming output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to MS_SMOOTH_GROUP_SETTINGS.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputGroupType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"Type of output group (File group, Apple HLS, DASH ISO, Microsoft Smooth Streaming, CMAF)\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: OutputGroupSettings
---

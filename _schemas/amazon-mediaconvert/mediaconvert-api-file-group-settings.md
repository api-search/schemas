---
description: Settings related to your File output group. MediaConvert uses this group of settings to generate a single standalone file, rather than a streaming package. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to FILE_GROUP_SETTINGS.
layout: schema
name: FileGroupSettings
properties_list:
- description: ''
  name: Destination
  type: object
- description: ''
  name: DestinationSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-file-group-settings-schema.json
slug: mediaconvert-api-file-group-settings
source_filename: mediaconvert-api-file-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-file-group-settings-schema.json\",\n  \"title\": \"FileGroupSettings\",\n  \"description\": \"Settings related to your File output group. MediaConvert uses this group of settings to generate a single standalone file, rather than a streaming package. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to FILE_GROUP_SETTINGS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"Use Destination (Destination) to specify the S3 output location and the output\
  \ filename base. Destination accepts format identifiers. If you do not specify the base filename in the URI, the service will use the filename of the input file. If your job has multiple inputs, the service uses the filename of the first input file.\"\n        }\n      ]\n    },\n    \"DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationSettings\"\n          },\n          \"description\": \"Settings associated with the destination. Will vary based on the type of destination\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-file-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: FileGroupSettings
---

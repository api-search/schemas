---
description: Settings specific to WebVTT sources in HLS alternative rendition group. Specify the properties (renditionGroupId, renditionName or renditionLanguageCode) to identify the unique subtitle track among the alternative rendition groups present in the HLS manifest. If no unique track is found, or multiple tracks match the specified properties, the job fails. If there is only one subtitle track in the rendition group, the settings can be left empty and the default subtitle track will be chosen. If your caption source is a sidecar file, use FileSourceSettings instead of WebvttHlsSourceSettings.
layout: schema
name: WebvttHlsSourceSettings
properties_list:
- description: ''
  name: RenditionGroupId
  type: object
- description: ''
  name: RenditionLanguageCode
  type: object
- description: ''
  name: RenditionName
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-webvtt-hls-source-settings-schema.json
slug: mediaconvert-api-webvtt-hls-source-settings
source_filename: mediaconvert-api-webvtt-hls-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-webvtt-hls-source-settings-schema.json\",\n  \"title\": \"WebvttHlsSourceSettings\",\n  \"description\": \"Settings specific to WebVTT sources in HLS alternative rendition group. Specify the properties (renditionGroupId, renditionName or renditionLanguageCode) to identify the unique subtitle track among the alternative rendition groups present in the HLS manifest. If no unique track is found, or multiple tracks match the specified properties, the job fails. If there is only one subtitle track in the rendition group, the settings can be left empty and the default subtitle track will be chosen. If your caption source is a sidecar file, use FileSourceSettings instead of WebvttHlsSourceSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RenditionGroupId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renditionGroupId\"\n          },\n          \"description\": \"Optional. Specify alternative group ID\"\n        }\n      ]\n    },\n    \"RenditionLanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renditionLanguageCode\"\n          },\n          \"description\": \"Optional. Specify ISO 639-2 or ISO 639-3 code in the language property\"\n        }\n      ]\n    },\n    \"RenditionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renditionName\"\n          },\n          \"description\": \"Optional. Specify media name\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-webvtt-hls-source-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: WebvttHlsSourceSettings
---

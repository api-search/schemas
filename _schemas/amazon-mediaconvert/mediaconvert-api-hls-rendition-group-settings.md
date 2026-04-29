---
description: Settings specific to audio sources in an HLS alternate rendition group. Specify the properties (renditionGroupId, renditionName or renditionLanguageCode) to identify the unique audio track among the alternative rendition groups present in the HLS manifest. If no unique track is found, or multiple tracks match the properties provided, the job fails. If no properties in hlsRenditionGroupSettings are specified, the default audio track within the video segment is chosen. If there is no audio within video segment, the alternative audio with DEFAULT=YES is chosen instead.
layout: schema
name: HlsRenditionGroupSettings
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
schema_file: json-schema/mediaconvert-api-hls-rendition-group-settings-schema.json
slug: mediaconvert-api-hls-rendition-group-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-rendition-group-settings-schema.json\",\n  \"title\": \"HlsRenditionGroupSettings\",\n  \"description\": \"Settings specific to audio sources in an HLS alternate rendition group. Specify the properties (renditionGroupId, renditionName or renditionLanguageCode) to identify the unique audio track among the alternative rendition groups present in the HLS manifest. If no unique track is found, or multiple tracks match the properties provided, the job fails. If no properties in hlsRenditionGroupSettings are specified, the default audio track within the video segment is chosen. If there is no audio within video segment, the alternative audio with DEFAULT=YES is chosen instead.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RenditionGroupId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renditionGroupId\"\n          },\n          \"description\": \"Optional. Specify alternative group ID\"\n        }\n      ]\n    },\n    \"RenditionLanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renditionLanguageCode\"\n          },\n          \"description\": \"Optional. Specify ISO 639-2 or ISO 639-3 code in the language property\"\n        }\n      ]\n    },\n    \"RenditionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renditionName\"\n          },\n          \"description\": \"Optional. Specify media name\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-rendition-group-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsRenditionGroupSettings
---

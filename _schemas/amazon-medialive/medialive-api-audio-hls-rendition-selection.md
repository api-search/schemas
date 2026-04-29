---
description: Audio Hls Rendition Selection
layout: schema
name: AudioHlsRenditionSelection
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-hls-rendition-selection-schema.json
slug: medialive-api-audio-hls-rendition-selection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-hls-rendition-selection-schema.json\",\n  \"title\": \"AudioHlsRenditionSelection\",\n  \"description\": \"Audio Hls Rendition Selection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groupId\"\n          },\n          \"description\": \"Specifies the GROUP-ID in the #EXT-X-MEDIA tag of the target HLS audio rendition.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Specifies the NAME in the #EXT-X-MEDIA\
  \ tag of the target HLS audio rendition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"GroupId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-hls-rendition-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioHlsRenditionSelection
---

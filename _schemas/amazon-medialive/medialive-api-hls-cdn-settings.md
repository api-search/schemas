---
description: Hls Cdn Settings
layout: schema
name: HlsCdnSettings
properties_list:
- description: ''
  name: HlsAkamaiSettings
  type: object
- description: ''
  name: HlsBasicPutSettings
  type: object
- description: ''
  name: HlsMediaStoreSettings
  type: object
- description: ''
  name: HlsS3Settings
  type: object
- description: ''
  name: HlsWebdavSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-cdn-settings-schema.json
slug: medialive-api-hls-cdn-settings
source_filename: medialive-api-hls-cdn-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-cdn-settings-schema.json\",\n  \"title\": \"HlsCdnSettings\",\n  \"description\": \"Hls Cdn Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HlsAkamaiSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsAkamaiSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsAkamaiSettings\"\n          }\n        }\n      ]\n    },\n    \"HlsBasicPutSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsBasicPutSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsBasicPutSettings\"\n          }\n        }\n      ]\n    },\n    \"HlsMediaStoreSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsMediaStoreSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsMediaStoreSettings\"\n          }\n        }\n      ]\n    },\n    \"HlsS3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsS3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsS3Settings\"\n          }\n        }\n      ]\n    },\n    \"HlsWebdavSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsWebdavSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsWebdavSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-cdn-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsCdnSettings
---

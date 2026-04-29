---
description: Hls Media Store Settings
layout: schema
name: HlsMediaStoreSettings
properties_list:
- description: ''
  name: ConnectionRetryInterval
  type: object
- description: ''
  name: FilecacheDuration
  type: object
- description: ''
  name: MediaStoreStorageClass
  type: object
- description: ''
  name: NumRetries
  type: object
- description: ''
  name: RestartDelay
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-media-store-settings-schema.json
slug: medialive-api-hls-media-store-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-media-store-settings-schema.json\",\n  \"title\": \"HlsMediaStoreSettings\",\n  \"description\": \"Hls Media Store Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionRetryInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectionRetryInterval\"\n          },\n          \"description\": \"Number of seconds to wait before retrying connection to the CDN if the connection is lost.\"\n        }\n      ]\n    },\n    \"FilecacheDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max600\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filecacheDuration\"\n          },\n\
  \          \"description\": \"Size in seconds of file cache for streaming outputs.\"\n        }\n      ]\n    },\n    \"MediaStoreStorageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsMediaStoreStorageClass\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStoreStorageClass\"\n          },\n          \"description\": \"When set to temporal, output files are stored in non-persistent memory for faster reading and writing.\"\n        }\n      ]\n    },\n    \"NumRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numRetries\"\n          },\n          \"description\": \"Number of retry attempts that will be made before the Live Event is put into an error state. Applies only if the CDN destination URI begins with \\\"s3\\\" or \\\"mediastore\\\". For other URIs, the value is always 3.\"\n        }\n   \
  \   ]\n    },\n    \"RestartDelay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max15\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"restartDelay\"\n          },\n          \"description\": \"If a streaming output fails, number of seconds to wait until a restart is initiated. A value of 0 means never restart.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-media-store-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsMediaStoreSettings
---

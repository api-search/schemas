---
description: Archive Group Settings
layout: schema
name: ArchiveGroupSettings
properties_list:
- description: ''
  name: ArchiveCdnSettings
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: RolloverInterval
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-archive-group-settings-schema.json
slug: medialive-api-archive-group-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-archive-group-settings-schema.json\",\n  \"title\": \"ArchiveGroupSettings\",\n  \"description\": \"Archive Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArchiveCdnSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchiveCdnSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"archiveCdnSettings\"\n          },\n          \"description\": \"Parameters that control interactions with the CDN.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"A directory and base filename where\
  \ archive files should be written.\"\n        }\n      ]\n    },\n    \"RolloverInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rolloverInterval\"\n          },\n          \"description\": \"Number of seconds to write to archive file before closing and starting a new one.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-archive-group-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ArchiveGroupSettings
---

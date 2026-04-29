---
description: Archive Cdn Settings
layout: schema
name: ArchiveCdnSettings
properties_list:
- description: ''
  name: ArchiveS3Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-archive-cdn-settings-schema.json
slug: medialive-api-archive-cdn-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-archive-cdn-settings-schema.json\",\n  \"title\": \"ArchiveCdnSettings\",\n  \"description\": \"Archive Cdn Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArchiveS3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchiveS3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"archiveS3Settings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-archive-cdn-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ArchiveCdnSettings
---

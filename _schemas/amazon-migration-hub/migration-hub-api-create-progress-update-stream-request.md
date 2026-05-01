---
description: CreateProgressUpdateStreamRequest schema from Amazon Migration Hub API
layout: schema
name: CreateProgressUpdateStreamRequest
properties_list:
- description: ''
  name: ProgressUpdateStreamName
  type: object
- description: ''
  name: DryRun
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-create-progress-update-stream-request-schema.json
slug: migration-hub-api-create-progress-update-stream-request
source_filename: migration-hub-api-create-progress-update-stream-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-create-progress-update-stream-request-schema.json\",\n  \"title\": \"CreateProgressUpdateStreamRequest\",\n  \"description\": \"CreateProgressUpdateStreamRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRun\"\n        },\n        {\n          \"description\": \"Optional boolean flag to indicate whether any effect should take place. Used to\
  \ test if the caller has permission to make the call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProgressUpdateStreamName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-create-progress-update-stream-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateProgressUpdateStreamRequest
---

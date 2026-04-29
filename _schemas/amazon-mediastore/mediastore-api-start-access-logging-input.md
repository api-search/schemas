---
description: StartAccessLoggingInput schema from Amazon MediaStore API
layout: schema
name: StartAccessLoggingInput
properties_list:
- description: ''
  name: ContainerName
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-start-access-logging-input-schema.json
slug: mediastore-api-start-access-logging-input
source_filename: mediastore-api-start-access-logging-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-start-access-logging-input-schema.json\",\n  \"title\": \"StartAccessLoggingInput\",\n  \"description\": \"StartAccessLoggingInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container that you want to start access logging on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-start-access-logging-input-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StartAccessLoggingInput
---

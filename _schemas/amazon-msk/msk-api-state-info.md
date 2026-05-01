---
description: StateInfo schema from Amazon MSK API
layout: schema
name: StateInfo
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-state-info-schema.json
slug: msk-api-state-info
source_filename: msk-api-state-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-state-info-schema.json\",\n  \"title\": \"StateInfo\",\n  \"description\": \"StateInfo schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"code\"\n          }\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"message\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-state-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: StateInfo
---

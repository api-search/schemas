---
description: Information about a tag.
layout: schema
name: Tag
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-tag-schema.json
slug: amazon-direct-connect-tag
source_filename: amazon-direct-connect-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Information about a tag.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"The key.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"The value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-tag-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: Tag
---

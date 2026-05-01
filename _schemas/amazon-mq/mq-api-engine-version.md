---
description: Id of the engine version.
layout: schema
name: EngineVersion
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-engine-version-schema.json
slug: mq-api-engine-version
source_filename: mq-api-engine-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-engine-version-schema.json\",\n  \"title\": \"EngineVersion\",\n  \"description\": \"Id of the engine version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Id for the version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-engine-version-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EngineVersion
---

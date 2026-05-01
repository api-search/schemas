---
description: KafkaVersion schema from Amazon MSK API
layout: schema
name: KafkaVersion
properties_list:
- description: ''
  name: Version
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-kafka-version-schema.json
slug: msk-api-kafka-version
source_filename: msk-api-kafka-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-kafka-version-schema.json\",\n  \"title\": \"KafkaVersion\",\n  \"description\": \"KafkaVersion schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"version\"\n          }\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KafkaVersionStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-kafka-version-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: KafkaVersion
---

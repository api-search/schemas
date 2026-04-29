---
description: GetCompatibleKafkaVersionsResponse schema from Amazon MSK API
layout: schema
name: GetCompatibleKafkaVersionsResponse
properties_list:
- description: ''
  name: CompatibleKafkaVersions
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-get-compatible-kafka-versions-response-schema.json
slug: msk-api-get-compatible-kafka-versions-response
source_filename: msk-api-get-compatible-kafka-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-get-compatible-kafka-versions-response-schema.json\",\n  \"title\": \"GetCompatibleKafkaVersionsResponse\",\n  \"description\": \"GetCompatibleKafkaVersionsResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompatibleKafkaVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCompatibleKafkaVersion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"compatibleKafkaVersions\"\n          },\n          \"description\": \"\\n            <p>A list of CompatibleKafkaVersion objects.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-get-compatible-kafka-versions-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetCompatibleKafkaVersionsResponse
---

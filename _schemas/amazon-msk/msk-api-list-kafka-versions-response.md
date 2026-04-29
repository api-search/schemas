---
description: ListKafkaVersionsResponse schema from Amazon MSK API
layout: schema
name: ListKafkaVersionsResponse
properties_list:
- description: ''
  name: KafkaVersions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-kafka-versions-response-schema.json
slug: msk-api-list-kafka-versions-response
source_filename: msk-api-list-kafka-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-kafka-versions-response-schema.json\",\n  \"title\": \"ListKafkaVersionsResponse\",\n  \"description\": \"ListKafkaVersionsResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KafkaVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfKafkaVersion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaVersions\"\n          }\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-kafka-versions-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListKafkaVersionsResponse
---

---
description: <p>Contains source Apache Kafka versions and compatible target Apache Kafka versions.</p>
layout: schema
name: CompatibleKafkaVersion
properties_list:
- description: ''
  name: SourceVersion
  type: object
- description: ''
  name: TargetVersions
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-compatible-kafka-version-schema.json
slug: msk-api-compatible-kafka-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-compatible-kafka-version-schema.json\",\n  \"title\": \"CompatibleKafkaVersion\",\n  \"description\": \"\\n            <p>Contains source Apache Kafka versions and compatible target Apache Kafka versions.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceVersion\"\n          },\n          \"description\": \"\\n            <p>An Apache Kafka version.</p>\"\n        }\n      ]\n    },\n    \"TargetVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetVersions\"\n          },\n         \
  \ \"description\": \"\\n            <p>A list of Apache Kafka versions.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-compatible-kafka-version-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CompatibleKafkaVersion
---

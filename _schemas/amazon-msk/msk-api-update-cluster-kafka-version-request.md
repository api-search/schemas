---
description: UpdateClusterKafkaVersionRequest schema from Amazon MSK API
layout: schema
name: UpdateClusterKafkaVersionRequest
properties_list:
- description: ''
  name: ConfigurationInfo
  type: object
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: TargetKafkaVersion
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-cluster-kafka-version-request-schema.json
slug: msk-api-update-cluster-kafka-version-request
source_filename: msk-api-update-cluster-kafka-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-cluster-kafka-version-request-schema.json\",\n  \"title\": \"UpdateClusterKafkaVersionRequest\",\n  \"description\": \"UpdateClusterKafkaVersionRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurationInfo\"\n          },\n          \"description\": \"\\n            <p>The custom configuration that should be applied on the new version of cluster.</p>\"\n        }\n      ]\n    },\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\
  \n          },\n          \"description\": \"\\n            <p>Current cluster version.</p>\"\n        }\n      ]\n    },\n    \"TargetKafkaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetKafkaVersion\"\n          },\n          \"description\": \"\\n            <p>Target Kafka version.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetKafkaVersion\",\n    \"CurrentVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-cluster-kafka-version-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateClusterKafkaVersionRequest
---

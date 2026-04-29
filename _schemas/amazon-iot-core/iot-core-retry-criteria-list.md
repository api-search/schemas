---
description: RetryCriteriaList schema
layout: schema
name: RetryCriteriaList
properties_list: []
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-retry-criteria-list-schema.json
slug: iot-core-retry-criteria-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-retry-criteria-list-schema.json\",\n  \"title\": \"RetryCriteriaList\",\n  \"description\": \"RetryCriteriaList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"failureType\",\n      \"numberOfRetries\"\n    ],\n    \"properties\": {\n      \"failureType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RetryableFailureType\"\n          },\n          {\n            \"description\": \"The type of job execution failures that can initiate a job retry.\"\n          }\n        ]\n      },\n      \"numberOfRetries\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NumberOfRetries\"\n          },\n          {\n            \"description\": \"The number of retries allowed for\
  \ a failure type for the job.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The criteria that determines how many retries are allowed for each failure type for a job.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-retry-criteria-list-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: RetryCriteriaList
---

---
description: An over-the-air firmware update job for FreeRTOS microcontroller devices.
layout: schema
name: OtaUpdate
properties_list:
- description: Unique OTA update identifier.
  name: otaUpdateId
  type: string
- description: ARN of the OTA update.
  name: otaUpdateArn
  type: string
- description: Current status of the OTA update.
  name: otaUpdateStatus
  type: string
- description: ''
  name: description
  type: string
- description: ARNs of target devices, things, or thing groups.
  name: targets
  type: array
- description: Delivery protocols (MQTT or HTTP).
  name: protocols
  type: array
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastModifiedDate
  type: string
- description: ''
  name: awsIotJobId
  type: string
- description: ''
  name: awsIotJobArn
  type: string
provider_name: Amazon FreeRTOS
provider_slug: amazon-freertos
schema_file: json-schema/amazon-freertos-ota-update-schema.json
slug: amazon-freertos-ota-update
source_filename: amazon-freertos-ota-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-ota-update-schema.json\",\n  \"title\": \"OtaUpdate\",\n  \"description\": \"An over-the-air firmware update job for FreeRTOS microcontroller devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"otaUpdateId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique OTA update identifier.\"\n    },\n    \"otaUpdateArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the OTA update.\"\n    },\n    \"otaUpdateStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_PENDING\",\n        \"CREATE_IN_PROGRESS\",\n        \"CREATE_COMPLETE\",\n        \"CREATE_FAILED\"\n      ],\n      \"description\": \"Current status of the OTA update.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"targets\": {\n      \"\
  type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"ARNs of target devices, things, or thing groups.\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Delivery protocols (MQTT or HTTP).\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"awsIotJobId\": {\n      \"type\": \"string\"\n    },\n    \"awsIotJobArn\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"otaUpdateId\",\n    \"targets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-ota-update-schema.json
tags:
- Embedded Systems
- IoT
- Microcontrollers
- RTOS
title: OtaUpdate
---

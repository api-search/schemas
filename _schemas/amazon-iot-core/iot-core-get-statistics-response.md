---
description: GetStatisticsResponse schema
layout: schema
name: GetStatisticsResponse
properties_list:
- description: ''
  name: statistics
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-statistics-response-schema.json
slug: iot-core-get-statistics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-statistics-response-schema.json\",\n  \"title\": \"GetStatisticsResponse\",\n  \"description\": \"GetStatisticsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Statistics\"\n        },\n        {\n          \"description\": \"The statistics returned by the Fleet Indexing service based on the query and aggregation field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-statistics-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: GetStatisticsResponse
---

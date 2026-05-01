---
description: GetStatisticsResponse schema
layout: schema
name: GetStatisticsResponse
properties_list:
- description: ''
  name: statistics
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-statistics-response-schema.json
slug: iot-device-management-get-statistics-response
source_filename: iot-device-management-get-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-statistics-response-schema.json\",\n  \"title\": \"GetStatisticsResponse\",\n  \"description\": \"GetStatisticsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Statistics\"\n        },\n        {\n          \"description\": \"The statistics returned by the Fleet Indexing service based on the query and aggregation field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-statistics-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetStatisticsResponse
---

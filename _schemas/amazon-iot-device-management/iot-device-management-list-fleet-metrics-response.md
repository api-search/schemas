---
description: ListFleetMetricsResponse schema
layout: schema
name: ListFleetMetricsResponse
properties_list:
- description: ''
  name: fleetMetrics
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-fleet-metrics-response-schema.json
slug: iot-device-management-list-fleet-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-fleet-metrics-response-schema.json\",\n  \"title\": \"ListFleetMetricsResponse\",\n  \"description\": \"ListFleetMetricsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricNameAndArnList\"\n        },\n        {\n          \"description\": \"The list of fleet metrics objects.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results. Will not be returned if the operation has returned all results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-fleet-metrics-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListFleetMetricsResponse
---

---
description: CreateFleetMetricResponse schema
layout: schema
name: CreateFleetMetricResponse
properties_list:
- description: ''
  name: metricName
  type: object
- description: ''
  name: metricArn
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-fleet-metric-response-schema.json
slug: iot-device-management-create-fleet-metric-response
source_filename: iot-device-management-create-fleet-metric-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-fleet-metric-response-schema.json\",\n  \"title\": \"CreateFleetMetricResponse\",\n  \"description\": \"CreateFleetMetricResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricName\"\n        },\n        {\n          \"description\": \"The name of the fleet metric to create.\"\n        }\n      ]\n    },\n    \"metricArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetMetricArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the new fleet metric.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-fleet-metric-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateFleetMetricResponse
---

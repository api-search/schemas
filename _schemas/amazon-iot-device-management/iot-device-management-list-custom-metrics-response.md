---
description: ListCustomMetricsResponse schema
layout: schema
name: ListCustomMetricsResponse
properties_list:
- description: ''
  name: metricNames
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-custom-metrics-response-schema.json
slug: iot-device-management-list-custom-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-custom-metrics-response-schema.json\",\n  \"title\": \"ListCustomMetricsResponse\",\n  \"description\": \"ListCustomMetricsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricNames\"\n        },\n        {\n          \"description\": \" The name of the custom metric. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-custom-metrics-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListCustomMetricsResponse
---

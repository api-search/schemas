---
description: ListMetricValuesResponse schema
layout: schema
name: ListMetricValuesResponse
properties_list:
- description: ''
  name: metricDatumList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-metric-values-response-schema.json
slug: iot-core-list-metric-values-response
source_filename: iot-core-list-metric-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-metric-values-response-schema.json\",\n  \"title\": \"ListMetricValuesResponse\",\n  \"description\": \"ListMetricValuesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricDatumList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDatumList\"\n        },\n        {\n          \"description\": \"The data the thing reports for the metric during the specified time period.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-metric-values-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListMetricValuesResponse
---

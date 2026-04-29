---
description: Contains asset property value information.
layout: schema
name: AssetPropertyValue
properties_list:
- description: ''
  name: value
  type: object
- description: ''
  name: timestamp
  type: object
- description: ''
  name: quality
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-property-value-schema.json
slug: iot-sitewise-asset-property-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-value-schema.json\",\n  \"title\": \"AssetPropertyValue\",\n  \"description\": \"Contains asset property value information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Variant\"\n        },\n        {\n          \"description\": \"The value of the asset property (see <code>Variant</code>).\"\n        }\n      ]\n    },\n    \"timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeInNanos\"\n        },\n        {\n          \"description\": \"The timestamp of the asset property value.\"\n        }\n      ]\n    },\n    \"quality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Quality\"\n        },\n      \
  \  {\n          \"description\": \"The quality of the asset property value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"value\",\n    \"timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-value-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetPropertyValue
---

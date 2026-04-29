---
description: PropertyFilters schema
layout: schema
name: PropertyFilters
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-filters-schema.json
slug: iot-twinmaker-property-filters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-filters-schema.json\",\n  \"title\": \"PropertyFilters\",\n  \"description\": \"PropertyFilters schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"propertyName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The property name associated with this property filter.\"\n          }\n        ]\n      },\n      \"operator\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The operator associated with this property filter.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n     \
  \       \"$ref\": \"#/components/schemas/DataValue\"\n          },\n          {\n            \"description\": \"The value associated with this property filter.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that filters items returned by a property request.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-filters-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyFilters
---

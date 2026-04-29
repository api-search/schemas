---
description: PropertyGroupsResponse schema
layout: schema
name: PropertyGroupsResponse
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-groups-response-schema.json
slug: iot-twinmaker-property-groups-response
source_filename: iot-twinmaker-property-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-groups-response-schema.json\",\n  \"title\": \"PropertyGroupsResponse\",\n  \"description\": \"PropertyGroupsResponse schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"groupType\",\n      \"propertyNames\",\n      \"isInherited\"\n    ],\n    \"properties\": {\n      \"groupType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/GroupType\"\n          },\n          {\n            \"description\": \"The group types.\"\n          }\n        ]\n      },\n      \"propertyNames\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyNames\"\n          },\n          {\n            \"description\": \"The names of properties.\"\n         \
  \ }\n        ]\n      },\n      \"isInherited\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value that specifies whether the property group is inherited from a parent entity\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The property group response\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-groups-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyGroupsResponse
---

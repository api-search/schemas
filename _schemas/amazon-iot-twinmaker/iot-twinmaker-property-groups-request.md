---
description: PropertyGroupsRequest schema
layout: schema
name: PropertyGroupsRequest
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-groups-request-schema.json
slug: iot-twinmaker-property-groups-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-groups-request-schema.json\",\n  \"title\": \"PropertyGroupsRequest\",\n  \"description\": \"PropertyGroupsRequest schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"groupType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/GroupType\"\n          },\n          {\n            \"description\": \"The group type.\"\n          }\n        ]\n      },\n      \"propertyNames\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyNames\"\n          },\n          {\n            \"description\": \"The names of properties.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"<p/>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-groups-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyGroupsRequest
---

---
description: <p/>
layout: schema
name: PropertyGroupRequest
properties_list:
- description: ''
  name: groupType
  type: object
- description: ''
  name: propertyNames
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-group-request-schema.json
slug: iot-twinmaker-property-group-request
source_filename: iot-twinmaker-property-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-group-request-schema.json\",\n  \"title\": \"PropertyGroupRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupType\"\n        },\n        {\n          \"description\": \"The group type.\"\n        }\n      ]\n    },\n    \"propertyNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyNames\"\n        },\n        {\n          \"description\": \"The names of properties.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-group-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyGroupRequest
---

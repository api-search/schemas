---
description: <p>An object that filters items in a list of component types.</p> <note> <p>Only one object is accepted as a valid input.</p> </note>
layout: schema
name: ListComponentTypesFilter
properties_list:
- description: ''
  name: extendsFrom
  type: object
- description: ''
  name: namespace
  type: object
- description: ''
  name: isAbstract
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-list-component-types-filter-schema.json
slug: iot-twinmaker-list-component-types-filter
source_filename: iot-twinmaker-list-component-types-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-component-types-filter-schema.json\",\n  \"title\": \"ListComponentTypesFilter\",\n  \"description\": \"<p>An object that filters items in a list of component types.</p> <note> <p>Only one object is accepted as a valid input.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"extendsFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n          \"description\": \"The component type that the component types in the list extend.\"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The namespace to which the component types in the list belong.\"\n        }\n \
  \     ]\n    },\n    \"isAbstract\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the component types in the list are abstract.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-list-component-types-filter-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ListComponentTypesFilter
---

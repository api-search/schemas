---
description: GetPropertyValueRequest schema
layout: schema
name: GetPropertyValueRequest
properties_list:
- description: ''
  name: componentName
  type: object
- description: ''
  name: componentTypeId
  type: object
- description: ''
  name: entityId
  type: object
- description: ''
  name: selectedProperties
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: propertyGroupName
  type: object
- description: ''
  name: tabularConditions
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-property-value-request-schema.json
slug: iot-twinmaker-get-property-value-request
source_filename: iot-twinmaker-get-property-value-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-property-value-request-schema.json\",\n  \"title\": \"GetPropertyValueRequest\",\n  \"description\": \"GetPropertyValueRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the component whose property values the operation returns.\"\n        }\n      ]\n    },\n    \"componentTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n          \"description\": \"The ID of the component type whose property values the operation returns.\"\n        }\n      ]\n    },\n    \"entityId\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the entity whose property values the operation returns.\"\n        }\n      ]\n    },\n    \"selectedProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelectedPropertyList\"\n        },\n        {\n          \"description\": \"The properties whose values the operation returns.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results to return at one time. The default is 25.</p> <p>Valid Range: Minimum value of 1. Maximum value of 250.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n\
  \        }\n      ]\n    },\n    \"propertyGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The property group name.\"\n        }\n      ]\n    },\n    \"tabularConditions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TabularConditions\"\n        },\n        {\n          \"description\": \"The tabular conditions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"selectedProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-property-value-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetPropertyValueRequest
---

---
description: GetPropertyValueHistoryRequest schema
layout: schema
name: GetPropertyValueHistoryRequest
properties_list:
- description: ''
  name: entityId
  type: object
- description: ''
  name: componentName
  type: object
- description: ''
  name: componentTypeId
  type: object
- description: ''
  name: selectedProperties
  type: object
- description: ''
  name: propertyFilters
  type: object
- description: ''
  name: startDateTime
  type: object
- description: ''
  name: endDateTime
  type: object
- description: ''
  name: interpolation
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: orderByTime
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-property-value-history-request-schema.json
slug: iot-twinmaker-get-property-value-history-request
source_filename: iot-twinmaker-get-property-value-history-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-property-value-history-request-schema.json\",\n  \"title\": \"GetPropertyValueHistoryRequest\",\n  \"description\": \"GetPropertyValueHistoryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the entity.\"\n        }\n      ]\n    },\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"componentTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n         \
  \ \"description\": \"The ID of the component type.\"\n        }\n      ]\n    },\n    \"selectedProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelectedPropertyList\"\n        },\n        {\n          \"description\": \"A list of properties whose value histories the request retrieves.\"\n        }\n      ]\n    },\n    \"propertyFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyFilters\"\n        },\n        {\n          \"description\": \"A list of objects that filter the property value history request.\"\n        }\n      ]\n    },\n    \"startDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The date and time of the earliest property value to return.This field is deprecated and will throw an error in the future. Use startTime instead.\"\n        }\n      ]\n  \
  \  },\n    \"endDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The date and time of the latest property value to return.This field is deprecated and will throw an error in the future. Use endTime instead.\"\n        }\n      ]\n    },\n    \"interpolation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterpolationParameters\"\n        },\n        {\n          \"description\": \"An object that specifies the interpolation type and the interval over which to interpolate data.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results to return at one time. The default is 25.</p> <p>Valid Range: Minimum value of 1. Maximum value of 250.</p>\"\n        }\n      ]\n    },\n    \"orderByTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderByTime\"\n        },\n        {\n          \"description\": \"The time direction to use in the result order.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"<p>The ISO8601 DateTime of the earliest property value to return.</p> <p>For more information about the ISO8601 DateTime format, see the data type <a href=\\\"https://docs.aws.amazon.com/iot-twinmaker/latest/apireference/API_PropertyValue.html\\\">PropertyValue</a>.</p>\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"<p>The ISO8601 DateTime of the latest property value to return.</p> <p>For more information about the ISO8601 DateTime format, see the data type <a href=\\\"https://docs.aws.amazon.com/iot-twinmaker/latest/apireference/API_PropertyValue.html\\\">PropertyValue</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"selectedProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-property-value-history-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetPropertyValueHistoryRequest
---

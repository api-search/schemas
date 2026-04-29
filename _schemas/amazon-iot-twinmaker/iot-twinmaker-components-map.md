---
description: ComponentsMap schema
layout: schema
name: ComponentsMap
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-components-map-schema.json
slug: iot-twinmaker-components-map
source_filename: iot-twinmaker-components-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-components-map-schema.json\",\n  \"title\": \"ComponentsMap\",\n  \"description\": \"ComponentsMap schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"componentName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the component.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\": \"The description of the component type.\"\n          }\n        ]\n      },\n      \"componentTypeId\": {\n        \"allOf\": [\n          {\n            \"$ref\"\
  : \"#/components/schemas/ComponentTypeId\"\n          },\n          {\n            \"description\": \"The ID of the component type.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Status\"\n          },\n          {\n            \"description\": \"The status of the component type.\"\n          }\n        ]\n      },\n      \"definedIn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The name of the property definition set in the request.\"\n          }\n        ]\n      },\n      \"properties\": {\n        \"description\": \"An object that maps strings to the properties to set in the component type. Each string in the mapping must be unique to this object.\"\n      },\n      \"propertyGroups\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentPropertyGroupResponses\"\
  \n          },\n          {\n            \"description\": \"The property groups.\"\n          }\n        ]\n      },\n      \"syncSource\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SyncSource\"\n          },\n          {\n            \"description\": \"The syncSource of the sync job, if this entity was created by a sync job.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that returns information about a component type create or update request.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-components-map-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ComponentsMap
---

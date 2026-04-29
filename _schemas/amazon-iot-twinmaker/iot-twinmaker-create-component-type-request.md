---
description: CreateComponentTypeRequest schema
layout: schema
name: CreateComponentTypeRequest
properties_list:
- description: ''
  name: isSingleton
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: propertyDefinitions
  type: object
- description: ''
  name: extendsFrom
  type: object
- description: ''
  name: functions
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: propertyGroups
  type: object
- description: ''
  name: componentTypeName
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-create-component-type-request-schema.json
slug: iot-twinmaker-create-component-type-request
source_filename: iot-twinmaker-create-component-type-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-component-type-request-schema.json\",\n  \"title\": \"CreateComponentTypeRequest\",\n  \"description\": \"CreateComponentTypeRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isSingleton\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether an entity can have more than one component of this type.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the component type.\"\n        }\n      ]\n    },\n    \"propertyDefinitions\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/PropertyDefinitionsRequest\"\n        },\n        {\n          \"description\": \"An object that maps strings to the property definitions in the component type. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"extendsFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExtendsFrom\"\n        },\n        {\n          \"description\": \"Specifies the parent component type to extend.\"\n        }\n      ]\n    },\n    \"functions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionsRequest\"\n        },\n        {\n          \"description\": \"An object that maps strings to the functions in the component type. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\":\
  \ \"Metadata that you can use to manage the component type.\"\n        }\n      ]\n    },\n    \"propertyGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyGroupsRequest\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"componentTypeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeName\"\n        },\n        {\n          \"description\": \"A friendly name for the component type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-create-component-type-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: CreateComponentTypeRequest
---

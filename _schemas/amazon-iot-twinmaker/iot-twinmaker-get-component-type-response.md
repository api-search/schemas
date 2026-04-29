---
description: GetComponentTypeResponse schema
layout: schema
name: GetComponentTypeResponse
properties_list:
- description: ''
  name: workspaceId
  type: object
- description: ''
  name: isSingleton
  type: object
- description: ''
  name: componentTypeId
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
  name: creationDateTime
  type: object
- description: ''
  name: updateDateTime
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: isAbstract
  type: object
- description: ''
  name: isSchemaInitialized
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: propertyGroups
  type: object
- description: ''
  name: syncSource
  type: object
- description: ''
  name: componentTypeName
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-component-type-response-schema.json
slug: iot-twinmaker-get-component-type-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-component-type-response-schema.json\",\n  \"title\": \"GetComponentTypeResponse\",\n  \"description\": \"GetComponentTypeResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the workspace that contains the component type.\"\n        }\n      ]\n    },\n    \"isSingleton\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether an entity can have more than one component of this type.\"\n        }\n      ]\n    },\n    \"componentTypeId\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ComponentTypeId\"\n        },\n        {\n          \"description\": \"The ID of the component type.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the component type.\"\n        }\n      ]\n    },\n    \"propertyDefinitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyDefinitionsResponse\"\n        },\n        {\n          \"description\": \"An object that maps strings to the property definitions in the component type. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"extendsFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExtendsFrom\"\n        },\n        {\n          \"description\": \"The name of the parent component type that this component type extends.\"\n    \
  \    }\n      ]\n    },\n    \"functions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionsResponse\"\n        },\n        {\n          \"description\": \"An object that maps strings to the functions in the component type. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"creationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the component type was created.\"\n        }\n      ]\n    },\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the component was last updated.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\"\
  : \"The ARN of the component type.\"\n        }\n      ]\n    },\n    \"isAbstract\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the component type is abstract.\"\n        }\n      ]\n    },\n    \"isSchemaInitialized\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the component type has a schema initializer and that the schema initializer has run.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The current status of the component type.\"\n        }\n      ]\n    },\n    \"propertyGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyGroupsResponse\"\
  \n        },\n        {\n          \"description\": \"<p>The maximum number of results to return at one time. The default is 25.</p> <p>Valid Range: Minimum value of 1. Maximum value of 250.</p>\"\n        }\n      ]\n    },\n    \"syncSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncSource\"\n        },\n        {\n          \"description\": \"The syncSource of the SyncJob, if this entity was created by a SyncJob.\"\n        }\n      ]\n    },\n    \"componentTypeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeName\"\n        },\n        {\n          \"description\": \"The component type name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"workspaceId\",\n    \"componentTypeId\",\n    \"creationDateTime\",\n    \"updateDateTime\",\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-component-type-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetComponentTypeResponse
---

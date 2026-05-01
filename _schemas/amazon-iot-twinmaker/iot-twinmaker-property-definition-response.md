---
description: An object that contains response data from a property definition request.
layout: schema
name: PropertyDefinitionResponse
properties_list:
- description: ''
  name: dataType
  type: object
- description: ''
  name: isTimeSeries
  type: object
- description: ''
  name: isRequiredInEntity
  type: object
- description: ''
  name: isExternalId
  type: object
- description: ''
  name: isStoredExternally
  type: object
- description: ''
  name: isImported
  type: object
- description: ''
  name: isFinal
  type: object
- description: ''
  name: isInherited
  type: object
- description: ''
  name: defaultValue
  type: object
- description: ''
  name: configuration
  type: object
- description: ''
  name: displayName
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-definition-response-schema.json
slug: iot-twinmaker-property-definition-response
source_filename: iot-twinmaker-property-definition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-definition-response-schema.json\",\n  \"title\": \"PropertyDefinitionResponse\",\n  \"description\": \"An object that contains response data from a property definition request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataType\"\n        },\n        {\n          \"description\": \"An object that contains information about the data type.\"\n        }\n      ]\n    },\n    \"isTimeSeries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the property consists of time series data.\"\n        }\n      ]\n    },\n    \"isRequiredInEntity\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the property is required in an entity.\"\n        }\n      ]\n    },\n    \"isExternalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the property ID comes from an external data store.\"\n        }\n      ]\n    },\n    \"isStoredExternally\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the property is stored externally.\"\n        }\n      ]\n    },\n    \"isImported\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the\
  \ property definition is imported from an external data store.\"\n        }\n      ]\n    },\n    \"isFinal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the property definition can be updated.\"\n        }\n      ]\n    },\n    \"isInherited\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the property definition is inherited from a parent entity.\"\n        }\n      ]\n    },\n    \"defaultValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValue\"\n        },\n        {\n          \"description\": \"An object that contains the default value.\"\n        }\n      ]\n    },\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Configuration\"\
  \n        },\n        {\n          \"description\": \"A mapping that specifies configuration information about the property.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyDisplayName\"\n        },\n        {\n          \"description\": \"A friendly name for the property.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dataType\",\n    \"isTimeSeries\",\n    \"isRequiredInEntity\",\n    \"isExternalId\",\n    \"isStoredExternally\",\n    \"isImported\",\n    \"isFinal\",\n    \"isInherited\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-definition-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyDefinitionResponse
---

---
description: PropertyDefinitionsRequest schema
layout: schema
name: PropertyDefinitionsRequest
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-definitions-request-schema.json
slug: iot-twinmaker-property-definitions-request
source_filename: iot-twinmaker-property-definitions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-definitions-request-schema.json\",\n  \"title\": \"PropertyDefinitionsRequest\",\n  \"description\": \"PropertyDefinitionsRequest schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"dataType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DataType\"\n          },\n          {\n            \"description\": \"An object that contains information about the data type.\"\n          }\n        ]\n      },\n      \"isRequiredInEntity\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value that specifies whether the property is required.\"\n          }\n       \
  \ ]\n      },\n      \"isExternalId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value that specifies whether the property ID comes from an external data store.\"\n          }\n        ]\n      },\n      \"isStoredExternally\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value that specifies whether the property is stored externally.\"\n          }\n        ]\n      },\n      \"isTimeSeries\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value that specifies whether the property consists of time series data.\"\n          }\n        ]\n      },\n      \"defaultValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DataValue\"\
  \n          },\n          {\n            \"description\": \"An object that contains the default value.\"\n          }\n        ]\n      },\n      \"configuration\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Configuration\"\n          },\n          {\n            \"description\": \"A mapping that specifies configuration information about the property. Use this field to specify information that you read from and write to an external source.\"\n          }\n        ]\n      },\n      \"displayName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyDisplayName\"\n          },\n          {\n            \"description\": \"A friendly name for the property.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that sets information about a property.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-definitions-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyDefinitionsRequest
---

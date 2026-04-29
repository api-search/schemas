---
description: Contains a subset of the possible runtime environment attributes. Used in the environment list.
layout: schema
name: EnvironmentSummary
properties_list:
- description: ''
  name: creationTime
  type: object
- description: ''
  name: engineType
  type: object
- description: ''
  name: engineVersion
  type: object
- description: ''
  name: environmentArn
  type: object
- description: ''
  name: environmentId
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-environment-summary-schema.json
slug: amazon-mainframe-modernization-environment-summary
source_filename: amazon-mainframe-modernization-environment-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-environment-summary-schema.json\",\n  \"title\": \"EnvironmentSummary\",\n  \"description\": \"Contains a subset of the possible runtime environment attributes. Used in the environment list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the runtime environment was created.\"\n        }\n      ]\n    },\n    \"engineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \"The target platform for the runtime environment.\"\n        }\n      ]\n    },\n    \"engineVersion\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineVersion\"\n        },\n        {\n          \"description\": \"The version of the runtime engine.\"\n        }\n      ]\n    },\n    \"environmentArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a particular runtime environment.\"\n        }\n      ]\n    },\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of a particular runtime environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n        {\n          \"description\": \"The instance type of the runtime environment.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the runtime environment.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentLifecycle\"\n        },\n        {\n          \"description\": \"The status of the runtime environment\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"creationTime\",\n    \"engineType\",\n    \"engineVersion\",\n    \"environmentArn\",\n    \"environmentId\",\n    \"instanceType\",\n    \"name\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-environment-summary-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: EnvironmentSummary
---

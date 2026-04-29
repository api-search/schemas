---
description: CreateEnvironmentRequest schema from AWS Mainframe Modernization API
layout: schema
name: CreateEnvironmentRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: engineType
  type: object
- description: ''
  name: engineVersion
  type: object
- description: ''
  name: highAvailabilityConfig
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: preferredMaintenanceWindow
  type: object
- description: ''
  name: publiclyAccessible
  type: object
- description: ''
  name: securityGroupIds
  type: object
- description: ''
  name: storageConfigurations
  type: object
- description: ''
  name: subnetIds
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-environment-request-schema.json
slug: amazon-mainframe-modernization-create-environment-request
source_filename: amazon-mainframe-modernization-create-environment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-environment-request-schema.json\",\n  \"title\": \"CreateEnvironmentRequest\",\n  \"description\": \"CreateEnvironmentRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier you provide to ensure the idempotency of the request to create an environment. The service generates the clientToken when the API call is triggered. The token expires after one hour, so if you retry the API within this timeframe with the same clientToken, you will get the same response. The service also handles deleting the clientToken after it\
  \ expires. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The description of the runtime environment.\"\n        }\n      ]\n    },\n    \"engineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \"The engine type for the runtime environment.\"\n        }\n      ]\n    },\n    \"engineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineVersion\"\n        },\n        {\n          \"description\": \"The version of the engine type for the runtime environment.\"\n        }\n      ]\n    },\n    \"highAvailabilityConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HighAvailabilityConfig\"\n        },\n        {\n          \"description\": \"The details of a high availability\
  \ configuration for this runtime environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n        {\n          \"description\": \"The type of instance for the runtime environment.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of a customer managed key.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the runtime environment. Must be unique within the account.\"\n        }\n      ]\n    },\n    \"preferredMaintenanceWindow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String50\"\n        },\n        {\n          \"description\": \"Configures the\
  \ maintenance window you want for the runtime environment. If you do not provide a value, a random system-generated value will be assigned.\"\n        }\n      ]\n    },\n    \"publiclyAccessible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the runtime environment is publicly accessible.\"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String50List\"\n        },\n        {\n          \"description\": \"The list of security groups for the VPC associated with this runtime environment.\"\n        }\n      ]\n    },\n    \"storageConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageConfigurationList\"\n        },\n        {\n          \"description\": \"Optional. The storage configurations for this runtime environment.\"\n        }\n      ]\n \
  \   },\n    \"subnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String50List\"\n        },\n        {\n          \"description\": \"The list of subnets associated with the VPC for this runtime environment.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags for the runtime environment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"engineType\",\n    \"instanceType\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-environment-request-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateEnvironmentRequest
---

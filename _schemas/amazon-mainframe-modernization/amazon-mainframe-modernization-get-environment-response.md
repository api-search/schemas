---
description: GetEnvironmentResponse schema from AWS Mainframe Modernization API
layout: schema
name: GetEnvironmentResponse
properties_list:
- description: ''
  name: actualCapacity
  type: object
- description: ''
  name: creationTime
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
  name: environmentArn
  type: object
- description: ''
  name: environmentId
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
  name: loadBalancerArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: pendingMaintenance
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
  name: status
  type: object
- description: ''
  name: statusReason
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
- description: ''
  name: vpcId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-get-environment-response-schema.json
slug: amazon-mainframe-modernization-get-environment-response
source_filename: amazon-mainframe-modernization-get-environment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-environment-response-schema.json\",\n  \"title\": \"GetEnvironmentResponse\",\n  \"description\": \"GetEnvironmentResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actualCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityValue\"\n        },\n        {\n          \"description\": \"The number of instances included in the runtime environment. A standalone runtime environment has a maxiumum of one instance. Currently, a high availability runtime environment has a maximum of two instances. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n\
  \          \"description\": \"The timestamp when the runtime environment was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The description of the runtime environment.\"\n        }\n      ]\n    },\n    \"engineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \"The target platform for the runtime environment.\"\n        }\n      ]\n    },\n    \"engineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineVersion\"\n        },\n        {\n          \"description\": \"The version of the runtime engine.\"\n        }\n      ]\n    },\n    \"environmentArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"\
  The Amazon Resource Name (ARN) of the runtime environment.\"\n        }\n      ]\n    },\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the runtime environment.\"\n        }\n      ]\n    },\n    \"highAvailabilityConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HighAvailabilityConfig\"\n        },\n        {\n          \"description\": \"The desired capacity of the high availability configuration for the runtime environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n        {\n          \"description\": \"The type of instance underlying the runtime environment.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n\
  \        },\n        {\n          \"description\": \"The identifier of a customer managed key.\"\n        }\n      ]\n    },\n    \"loadBalancerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the load balancer used with the runtime environment.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The name of the runtime environment. Must be unique within the account.\"\n        }\n      ]\n    },\n    \"pendingMaintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PendingMaintenance\"\n        },\n        {\n          \"description\": \"Indicates the pending maintenance scheduled on this environment.\"\n        }\n      ]\n    },\n    \"preferredMaintenanceWindow\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/String50\"\n        },\n        {\n          \"description\": \"Configures the maintenance window you want for the runtime environment. If you do not provide a value, a random system-generated value will be assigned.\"\n        }\n      ]\n    },\n    \"publiclyAccessible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether applications running in this runtime environment are publicly accessible. \"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String50List\"\n        },\n        {\n          \"description\": \"The unique identifiers of the security groups assigned to this runtime environment.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentLifecycle\"\n       \
  \ },\n        {\n          \"description\": \"The status of the runtime environment.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for the reported status.\"\n        }\n      ]\n    },\n    \"storageConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageConfigurationList\"\n        },\n        {\n          \"description\": \"The storage configurations defined for the runtime environment.\"\n        }\n      ]\n    },\n    \"subnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String50List\"\n        },\n        {\n          \"description\": \"The unique identifiers of the subnets assigned to this runtime environment.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n\
  \        },\n        {\n          \"description\": \"The tags defined for this runtime environment.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String50\"\n        },\n        {\n          \"description\": \"The unique identifier for the VPC used with this runtime environment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"creationTime\",\n    \"engineType\",\n    \"engineVersion\",\n    \"environmentArn\",\n    \"environmentId\",\n    \"instanceType\",\n    \"name\",\n    \"securityGroupIds\",\n    \"status\",\n    \"subnetIds\",\n    \"vpcId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-environment-response-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GetEnvironmentResponse
---

---
description: Contains details about the analyzed resource.
layout: schema
name: AnalyzedResource
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: analyzedAt
  type: object
- description: ''
  name: updatedAt
  type: object
- description: ''
  name: isPublic
  type: object
- description: ''
  name: actions
  type: object
- description: ''
  name: sharedVia
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: resourceOwnerAccount
  type: object
- description: ''
  name: error
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-analyzed-resource-schema.json
slug: iam-access-analyzer-analyzed-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzed-resource-schema.json\",\n  \"title\": \"AnalyzedResource\",\n  \"description\": \"Contains details about the analyzed resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The ARN of the resource that was analyzed.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of the resource that was analyzed.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n    \
  \    },\n        {\n          \"description\": \"The time at which the finding was created.\"\n        }\n      ]\n    },\n    \"analyzedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the resource was analyzed.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the finding was updated.\"\n        }\n      ]\n    },\n    \"isPublic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the policy that generated the finding grants public access to the resource.\"\n        }\n      ]\n    },\n    \"actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionList\"\n        },\n\
  \        {\n          \"description\": \"The actions that an external principal is granted permission to use by the policy that generated the finding.\"\n        }\n      ]\n    },\n    \"sharedVia\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SharedViaList\"\n        },\n        {\n          \"description\": \"Indicates how the access that generated the finding is granted. This is populated for Amazon S3 bucket findings.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingStatus\"\n        },\n        {\n          \"description\": \"The current status of the finding generated from the analyzed resource.\"\n        }\n      ]\n    },\n    \"resourceOwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID that owns the resource.\"\n        }\n \
  \     ]\n    },\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\",\n    \"resourceType\",\n    \"createdAt\",\n    \"analyzedAt\",\n    \"updatedAt\",\n    \"isPublic\",\n    \"resourceOwnerAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzed-resource-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: AnalyzedResource
---

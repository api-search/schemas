---
description: The resource filter criteria for a Software bill of materials (SBOM) report.
layout: schema
name: ResourceFilterCriteria
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: ec2InstanceTags
  type: object
- description: ''
  name: ecrImageTags
  type: object
- description: ''
  name: ecrRepositoryName
  type: object
- description: ''
  name: lambdaFunctionName
  type: object
- description: ''
  name: lambdaFunctionTags
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: resourceType
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-resource-filter-criteria-schema.json
slug: inspector-resource-filter-criteria
source_filename: inspector-resource-filter-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-filter-criteria-schema.json\",\n  \"title\": \"ResourceFilterCriteria\",\n  \"description\": \"The resource filter criteria for a Software bill of materials (SBOM) report.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStringFilterList\"\n        },\n        {\n          \"description\": \"The account IDs used as resource filter criteria.\"\n        }\n      ]\n    },\n    \"ec2InstanceTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceMapFilterList\"\n        },\n        {\n          \"description\": \"The EC2 instance tags used as resource filter criteria.\"\n        }\n      ]\n    },\n    \"ecrImageTags\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/ResourceStringFilterList\"\n        },\n        {\n          \"description\": \"The ECR image tags used as resource filter criteria.\"\n        }\n      ]\n    },\n    \"ecrRepositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStringFilterList\"\n        },\n        {\n          \"description\": \"The ECR repository names used as resource filter criteria.\"\n        }\n      ]\n    },\n    \"lambdaFunctionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStringFilterList\"\n        },\n        {\n          \"description\": \"The AWS Lambda function name used as resource filter criteria.\"\n        }\n      ]\n    },\n    \"lambdaFunctionTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceMapFilterList\"\n        },\n        {\n          \"description\": \"The AWS Lambda function tags used as resource filter\
  \ criteria.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStringFilterList\"\n        },\n        {\n          \"description\": \"The resource IDs used as resource filter criteria.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStringFilterList\"\n        },\n        {\n          \"description\": \"The resource types used as resource filter criteria.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-filter-criteria-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ResourceFilterCriteria
---

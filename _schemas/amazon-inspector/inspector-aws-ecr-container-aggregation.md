---
description: An aggregation of information about Amazon ECR containers.
layout: schema
name: AwsEcrContainerAggregation
properties_list:
- description: ''
  name: architectures
  type: object
- description: ''
  name: imageShas
  type: object
- description: ''
  name: imageTags
  type: object
- description: ''
  name: repositories
  type: object
- description: ''
  name: resourceIds
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-aws-ecr-container-aggregation-schema.json
slug: inspector-aws-ecr-container-aggregation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ecr-container-aggregation-schema.json\",\n  \"title\": \"AwsEcrContainerAggregation\",\n  \"description\": \"An aggregation of information about Amazon ECR containers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"architectures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The architecture of the containers.\"\n        }\n      ]\n    },\n    \"imageShas\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The image SHA values.\"\n        }\n      ]\n    },\n    \"imageTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n   \
  \     },\n        {\n          \"description\": \"The image tags.\"\n        }\n      ]\n    },\n    \"repositories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The container repositories.\"\n        }\n      ]\n    },\n    \"resourceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The container resource IDs.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsEcrContainerSortBy\"\n        },\n        {\n          \"description\": \"The value to sort by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The sort order (ascending or descending).\"\n        }\n   \
  \   ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ecr-container-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AwsEcrContainerAggregation
---

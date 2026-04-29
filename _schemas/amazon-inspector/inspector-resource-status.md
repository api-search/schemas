---
description: Details the status of Amazon Inspector for each resource type Amazon Inspector scans.
layout: schema
name: ResourceStatus
properties_list:
- description: ''
  name: ec2
  type: object
- description: ''
  name: ecr
  type: object
- description: ''
  name: lambda
  type: object
- description: ''
  name: lambdaCode
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-resource-status-schema.json
slug: inspector-resource-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-status-schema.json\",\n  \"title\": \"ResourceStatus\",\n  \"description\": \"Details the status of Amazon Inspector for each resource type Amazon Inspector scans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ec2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of Amazon Inspector scanning for Amazon EC2 resources.\"\n        }\n      ]\n    },\n    \"ecr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of Amazon Inspector scanning for Amazon ECR resources.\"\n        }\n      ]\n    },\n    \"lambda\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\
  \n        },\n        {\n          \"description\": \"The status of Amazon Inspector scanning for AWS Lambda function.\"\n        }\n      ]\n    },\n    \"lambdaCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"The status of Amazon Inspector scanning for custom application code for Amazon Web Services Lambda functions. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ec2\",\n    \"ecr\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-status-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ResourceStatus
---

---
description: An object that contains details about the metadata for an Amazon ECR resource.
layout: schema
name: ResourceScanMetadata
properties_list:
- description: ''
  name: ec2
  type: object
- description: ''
  name: ecrImage
  type: object
- description: ''
  name: ecrRepository
  type: object
- description: ''
  name: lambdaFunction
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-resource-scan-metadata-schema.json
slug: inspector-resource-scan-metadata
source_filename: inspector-resource-scan-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-scan-metadata-schema.json\",\n  \"title\": \"ResourceScanMetadata\",\n  \"description\": \"An object that contains details about the metadata for an Amazon ECR resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ec2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2Metadata\"\n        },\n        {\n          \"description\": \"An object that contains metadata details for an Amazon EC2 instance.\"\n        }\n      ]\n    },\n    \"ecrImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcrContainerImageMetadata\"\n        },\n        {\n          \"description\": \"An object that contains details about the container metadata for an Amazon ECR image.\"\n        }\n      ]\n    },\n    \"ecrRepository\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcrRepositoryMetadata\"\n        },\n        {\n          \"description\": \"An object that contains details about the repository an Amazon ECR image resides in.\"\n        }\n      ]\n    },\n    \"lambdaFunction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionMetadata\"\n        },\n        {\n          \"description\": \"An object that contains metadata details for an AWS Lambda function.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-resource-scan-metadata-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ResourceScanMetadata
---

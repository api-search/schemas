---
description: Contains details of the Amazon S3 bucket and KMS key used to export findings.
layout: schema
name: Destination
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: keyPrefix
  type: object
- description: ''
  name: kmsKeyArn
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-destination-schema.json
slug: inspector-destination
source_filename: inspector-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-destination-schema.json\",\n  \"title\": \"Destination\",\n  \"description\": \"Contains details of the Amazon S3 bucket and KMS key used to export findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket to export findings to.\"\n        }\n      ]\n    },\n    \"keyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The prefix that the findings will be written under.\"\n        }\n      ]\n    },\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n\
  \        },\n        {\n          \"description\": \"The ARN of the KMS key used to encrypt data when exporting findings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketName\",\n    \"kmsKeyArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-destination-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Destination
---

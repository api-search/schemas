---
description: Starts a scan of the policies applied to the specified resource.
layout: schema
name: StartResourceScanRequest
properties_list:
- description: ''
  name: analyzerArn
  type: object
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: resourceOwnerAccount
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-start-resource-scan-request-schema.json
slug: iam-access-analyzer-start-resource-scan-request
source_filename: iam-access-analyzer-start-resource-scan-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-start-resource-scan-request-schema.json\",\n  \"title\": \"StartResourceScanRequest\",\n  \"description\": \"Starts a scan of the policies applied to the specified resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-getting-started.html#permission-resources\\\">ARN of the analyzer</a> to use to scan the policies applied to the specified resource.\"\n        }\n      ]\n    },\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"\
  description\": \"The ARN of the resource to scan.\"\n        }\n      ]\n    },\n    \"resourceOwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID that owns the resource. For most Amazon Web Services resources, the owning account is the account in which the resource was created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzerArn\",\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-start-resource-scan-request-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: StartResourceScanRequest
---

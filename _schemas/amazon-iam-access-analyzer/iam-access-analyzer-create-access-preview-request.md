---
description: CreateAccessPreviewRequest schema from AWS IAM Access Analyzer API
layout: schema
name: CreateAccessPreviewRequest
properties_list:
- description: ''
  name: analyzerArn
  type: object
- description: ''
  name: configurations
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-create-access-preview-request-schema.json
slug: iam-access-analyzer-create-access-preview-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-access-preview-request-schema.json\",\n  \"title\": \"CreateAccessPreviewRequest\",\n  \"description\": \"CreateAccessPreviewRequest schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-getting-started.html#permission-resources\\\">ARN of the account analyzer</a> used to generate the access preview. You can only create an access preview for analyzers with an <code>Account</code> type and <code>Active</code> status.\"\n        }\n      ]\n    },\n    \"configurations\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationsMap\"\n        },\n        {\n          \"description\": \"Access control configuration for your resource that is used to generate the access preview. The access preview includes findings for external access allowed to the resource with the proposed access control configuration. The configuration must contain exactly one element.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A client token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzerArn\",\n    \"configurations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-create-access-preview-request-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: CreateAccessPreviewRequest
---

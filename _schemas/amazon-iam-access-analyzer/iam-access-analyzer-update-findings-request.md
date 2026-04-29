---
description: Updates findings with the new values provided in the request.
layout: schema
name: UpdateFindingsRequest
properties_list:
- description: ''
  name: analyzerArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: ids
  type: object
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-update-findings-request-schema.json
slug: iam-access-analyzer-update-findings-request
source_filename: iam-access-analyzer-update-findings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-update-findings-request-schema.json\",\n  \"title\": \"UpdateFindingsRequest\",\n  \"description\": \"Updates findings with the new values provided in the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-getting-started.html#permission-resources\\\">ARN of the analyzer</a> that generated the findings to update.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingStatusUpdate\"\n        },\n        {\n          \"description\": \"The state represents\
  \ the action to take to update the finding Status. Use <code>ARCHIVE</code> to change an Active finding to an Archived finding. Use <code>ACTIVE</code> to change an Archived finding to an Active finding.\"\n        }\n      ]\n    },\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingIdList\"\n        },\n        {\n          \"description\": \"The IDs of the findings to update.\"\n        }\n      ]\n    },\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The ARN of the resource identified in the finding.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A client token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzerArn\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-update-findings-request-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: UpdateFindingsRequest
---

---
description: Contains a summary of information about an access preview.
layout: schema
name: AccessPreviewSummary
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: analyzerArn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: status
  type: object
- description: 'Provides more details about the current status of the access preview. For example, if the creation of the access preview fails, a <code>Failed</code> status is returned. This failure can be due to an '
  name: statusReason
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-access-preview-summary-schema.json
slug: iam-access-analyzer-access-preview-summary
source_filename: iam-access-analyzer-access-preview-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-access-preview-summary-schema.json\",\n  \"title\": \"AccessPreviewSummary\",\n  \"description\": \"Contains a summary of information about an access preview.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreviewId\"\n        },\n        {\n          \"description\": \"The unique ID for the access preview.\"\n        }\n      ]\n    },\n    \"analyzerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The ARN of the analyzer used to generate the access preview.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time at which the access preview was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreviewStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the access preview.</p> <ul> <li> <p> <code>Creating</code> - The access preview creation is in progress.</p> </li> <li> <p> <code>Completed</code> - The access preview is complete and previews the findings for external access to the resource.</p> </li> <li> <p> <code>Failed</code> - The access preview creation has failed.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"code\"\n      ],\n      \"properties\": {\n        \"code\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/AccessPreviewStatusReasonCode\"\n            },\n            {\n      \
  \        \"description\": \"The reason code for the current status of the access preview.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Provides more details about the current status of the access preview. For example, if the creation of the access preview fails, a <code>Failed</code> status is returned. This failure can be due to an internal issue with the analysis or due to an invalid proposed resource configuration.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"analyzerArn\",\n    \"createdAt\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-access-preview-summary-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: AccessPreviewSummary
---

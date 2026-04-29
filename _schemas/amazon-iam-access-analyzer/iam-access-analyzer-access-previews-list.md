---
description: AccessPreviewsList schema from AWS IAM Access Analyzer API
layout: schema
name: AccessPreviewsList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-access-previews-list-schema.json
slug: iam-access-analyzer-access-previews-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-access-previews-list-schema.json\",\n  \"title\": \"AccessPreviewsList\",\n  \"description\": \"AccessPreviewsList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"id\",\n      \"analyzerArn\",\n      \"createdAt\",\n      \"status\"\n    ],\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccessPreviewId\"\n          },\n          {\n            \"description\": \"The unique ID for the access preview.\"\n          }\n        ]\n      },\n      \"analyzerArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AnalyzerArn\"\n          },\n          {\n            \"description\"\
  : \"The ARN of the analyzer used to generate the access preview.\"\n          }\n        ]\n      },\n      \"createdAt\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time at which the access preview was created.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccessPreviewStatus\"\n          },\n          {\n            \"description\": \"<p>The status of the access preview.</p> <ul> <li> <p> <code>Creating</code> - The access preview creation is in progress.</p> </li> <li> <p> <code>Completed</code> - The access preview is complete and previews the findings for external access to the resource.</p> </li> <li> <p> <code>Failed</code> - The access preview creation has failed.</p> </li> </ul>\"\n          }\n        ]\n      },\n      \"statusReason\": {\n        \"$ref\": \"#/components/schemas/AccessPreviewStatusReason\"\
  \n      }\n    },\n    \"description\": \"Contains a summary of information about an access preview.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-access-previews-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: AccessPreviewsList
---

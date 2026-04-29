---
description: AnalyzersList schema from AWS IAM Access Analyzer API
layout: schema
name: AnalyzersList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-analyzers-list-schema.json
slug: iam-access-analyzer-analyzers-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzers-list-schema.json\",\n  \"title\": \"AnalyzersList\",\n  \"description\": \"AnalyzersList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"arn\",\n      \"name\",\n      \"type\",\n      \"createdAt\",\n      \"status\"\n    ],\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AnalyzerArn\"\n          },\n          {\n            \"description\": \"The ARN of the analyzer.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Name\"\n          },\n          {\n            \"description\": \"The name of the analyzer.\"\n  \
  \        }\n        ]\n      },\n      \"type\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Type\"\n          },\n          {\n            \"description\": \"The type of analyzer, which corresponds to the zone of trust chosen for the analyzer.\"\n          }\n        ]\n      },\n      \"createdAt\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"A timestamp for the time at which the analyzer was created.\"\n          }\n        ]\n      },\n      \"lastResourceAnalyzed\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"The resource that was most recently analyzed by the analyzer.\"\n          }\n        ]\n      },\n      \"lastResourceAnalyzedAt\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\
  \n          },\n          {\n            \"description\": \"The time at which the most recently analyzed resource was analyzed.\"\n          }\n        ]\n      },\n      \"tags\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagsMap\"\n          },\n          {\n            \"description\": \"The tags added to the analyzer.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AnalyzerStatus\"\n          },\n          {\n            \"description\": \"The status of the analyzer. An <code>Active</code> analyzer successfully monitors supported resources and generates new findings. The analyzer is <code>Disabled</code> when a user action, such as removing trusted access for Identity and Access Management Access Analyzer from Organizations, causes the analyzer to stop generating new findings. The status is <code>Creating</code> when the analyzer creation is in progress\
  \ and <code>Failed</code> when the analyzer creation has failed. \"\n          }\n        ]\n      },\n      \"statusReason\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StatusReason\"\n          },\n          {\n            \"description\": \"The <code>statusReason</code> provides more details about the current status of the analyzer. For example, if the creation for the analyzer fails, a <code>Failed</code> status is returned. For an analyzer with organization as the type, this failure can be due to an issue with creating the service-linked roles required in the member accounts of the Amazon Web Services organization.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about the analyzer.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-analyzers-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: AnalyzersList
---

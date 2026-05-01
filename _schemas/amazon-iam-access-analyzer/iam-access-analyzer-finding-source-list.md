---
description: FindingSourceList schema from AWS IAM Access Analyzer API
layout: schema
name: FindingSourceList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-finding-source-list-schema.json
slug: iam-access-analyzer-finding-source-list
source_filename: iam-access-analyzer-finding-source-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-finding-source-list-schema.json\",\n  \"title\": \"FindingSourceList\",\n  \"description\": \"FindingSourceList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"type\"\n    ],\n    \"properties\": {\n      \"type\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FindingSourceType\"\n          },\n          {\n            \"description\": \"Indicates the type of access that generated the finding.\"\n          }\n        ]\n      },\n      \"detail\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FindingSourceDetail\"\n          },\n          {\n            \"description\": \"Includes details about how the access\
  \ that generated the finding is granted. This is populated for Amazon S3 bucket findings.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The source of the finding. This indicates how the access that generated the finding is granted. It is populated for Amazon S3 bucket findings.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-finding-source-list-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: FindingSourceList
---

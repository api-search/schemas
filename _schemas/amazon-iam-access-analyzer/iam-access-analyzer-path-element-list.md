---
description: PathElementList schema from AWS IAM Access Analyzer API
layout: schema
name: PathElementList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-path-element-list-schema.json
slug: iam-access-analyzer-path-element-list
source_filename: iam-access-analyzer-path-element-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-path-element-list-schema.json\",\n  \"title\": \"PathElementList\",\n  \"description\": \"PathElementList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"index\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Integer\"\n          },\n          {\n            \"description\": \"Refers to an index in a JSON array.\"\n          }\n        ]\n      },\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"Refers to a key in a JSON object.\"\n          }\n        ]\n      },\n      \"substring\": {\n        \"allOf\": [\n          {\n   \
  \         \"$ref\": \"#/components/schemas/Substring\"\n          },\n          {\n            \"description\": \"Refers to a substring of a literal string in a JSON object.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"Refers to the value associated with a given key in a JSON object.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A single element in a path through the JSON representation of a policy.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-path-element-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: PathElementList
---

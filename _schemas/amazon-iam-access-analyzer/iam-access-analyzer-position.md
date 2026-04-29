---
description: A position in a policy.
layout: schema
name: Position
properties_list:
- description: ''
  name: line
  type: object
- description: ''
  name: column
  type: object
- description: ''
  name: offset
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-position-schema.json
slug: iam-access-analyzer-position
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-position-schema.json\",\n  \"title\": \"Position\",\n  \"description\": \"A position in a policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The line of the position, starting from 1.\"\n        }\n      ]\n    },\n    \"column\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The column of the position, starting from 0.\"\n        }\n      ]\n    },\n    \"offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The offset within\
  \ the policy that corresponds to the position, starting from 0.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"line\",\n    \"column\",\n    \"offset\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-position-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: Position
---

---
description: The criteria used to sort.
layout: schema
name: SortCriteria
properties_list:
- description: ''
  name: attributeName
  type: object
- description: ''
  name: orderBy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-sort-criteria-schema.json
slug: iam-access-analyzer-sort-criteria
source_filename: iam-access-analyzer-sort-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-sort-criteria-schema.json\",\n  \"title\": \"SortCriteria\",\n  \"description\": \"The criteria used to sort.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the attribute to sort on.\"\n        }\n      ]\n    },\n    \"orderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\n        },\n        {\n          \"description\": \"The sort order, ascending or descending.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-sort-criteria-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: SortCriteria
---

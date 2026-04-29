---
description: Information about a filter used to limit results of a query.
layout: schema
name: Filter
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: values
  type: object
- description: ''
  name: comparisonOperator
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-filter-schema.json
slug: amazon-codecatalyst-filter
source_filename: amazon-codecatalyst-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Information about a filter used to limit results of a query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A key that can be used to sort results.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The values of the key.\"\n        }\n      ]\n    },\n    \"comparisonOperator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The operator\
  \ used to compare the fields.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-filter-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: Filter
---

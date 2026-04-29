---
description: CreateFilterRequest schema
layout: schema
name: CreateFilterRequest
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: filterCriteria
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: reason
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-create-filter-request-schema.json
slug: inspector-create-filter-request
source_filename: inspector-create-filter-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-create-filter-request-schema.json\",\n  \"title\": \"CreateFilterRequest\",\n  \"description\": \"CreateFilterRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterAction\"\n        },\n        {\n          \"description\": \"Defines the action that is to be applied to the findings that match the filter.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterDescription\"\n        },\n        {\n          \"description\": \"A description of the filter.\"\n        }\n      ]\n    },\n    \"filterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteria\"\n    \
  \    },\n        {\n          \"description\": \"Defines the criteria to be used in the filter for querying findings.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterName\"\n        },\n        {\n          \"description\": \"The name of the filter. Minimum length of 3. Maximum length of 64. Valid characters include alphanumeric characters, dot (.), underscore (_), and dash (-). Spaces are not allowed.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterReason\"\n        },\n        {\n          \"description\": \"The reason for creating the filter.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of tags for the filter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\",\n\
  \    \"filterCriteria\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-create-filter-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CreateFilterRequest
---

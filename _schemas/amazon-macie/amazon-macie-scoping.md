---
description: Specifies one or more property- and tag-based conditions that define criteria for including or excluding S3 objects from a classification job. Exclude conditions take precedence over include conditions.
layout: schema
name: Scoping
properties_list:
- description: ''
  name: excludes
  type: object
- description: ''
  name: includes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-scoping-schema.json
slug: amazon-macie-scoping
source_filename: amazon-macie-scoping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-scoping-schema.json\",\n  \"title\": \"Scoping\",\n  \"description\": \"Specifies one or more property- and tag-based conditions that define criteria for including or excluding S3 objects from a classification job. Exclude conditions take precedence over include conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobScopingBlock\"\n        },\n        {\n          \"description\": \"The property- and tag-based conditions that determine which objects to exclude from the analysis.\"\n        }\n      ]\n    },\n    \"includes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobScopingBlock\"\n        },\n        {\n          \"description\": \"The property- and\
  \ tag-based conditions that determine which objects to include in the analysis.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-scoping-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Scoping
---

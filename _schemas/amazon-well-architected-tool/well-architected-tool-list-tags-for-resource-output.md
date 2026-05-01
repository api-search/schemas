---
description: ListTagsForResourceOutput schema from AWS Well-Architected Tool API
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-tags-for-resource-output-schema.json
slug: well-architected-tool-list-tags-for-resource-output
source_filename: well-architected-tool-list-tags-for-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags for the resource.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-tags-for-resource-output-schema.json\",\n  \"description\": \"ListTagsForResourceOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-tags-for-resource-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListTagsForResourceOutput
---

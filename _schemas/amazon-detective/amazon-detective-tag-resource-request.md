---
description: Request to apply tags to a behavior graph
layout: schema
name: TagResourceRequest
properties_list:
- description: The tags to assign to the behavior graph.
  name: Tags
  type: object
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-tag-resource-request-schema.json
slug: amazon-detective-tag-resource-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"Request to apply tags to a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags to assign to the behavior graph.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-tag-resource-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: TagResourceRequest
---

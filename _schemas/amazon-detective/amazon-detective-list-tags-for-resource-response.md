---
description: Response from listing tags for a resource
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: The tag values that are assigned to the behavior graph.
  name: Tags
  type: object
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-tags-for-resource-response-schema.json
slug: amazon-detective-list-tags-for-resource-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"Response from listing tags for a resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tag values that are assigned to the behavior graph.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-tags-for-resource-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListTagsForResourceResponse
---

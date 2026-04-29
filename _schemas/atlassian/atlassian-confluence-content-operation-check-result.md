---
description: An operation and the target entity that it applies to, e.g. create page.
layout: schema
name: OperationCheckResult
properties_list:
- description: The operation itself.
  name: operation
  type: string
- description: The space or content type that the operation applies to. Could be one of- - application - page - blogpost - comment - attachment - space
  name: targetType
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-operation-check-result-schema.json
slug: atlassian-confluence-content-operation-check-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationCheckResult\",\n  \"type\": \"object\",\n  \"description\": \"An operation and the target entity that it applies to, e.g. create page.\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The operation itself.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"The space or content type that the operation applies to. Could be one of- - application - page - blogpost - comment - attachment - space\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-operation-check-result-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: OperationCheckResult
---

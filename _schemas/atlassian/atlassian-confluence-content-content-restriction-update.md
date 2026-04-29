---
description: ''
layout: schema
name: ContentRestrictionUpdate
properties_list:
- description: The restriction operation applied to content.
  name: operation
  type: string
- description: The users/groups that the restrictions will be applied to. At least one of `user` or `group` must be specified for this object.
  name: restrictions
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-restriction-update-schema.json
slug: atlassian-confluence-content-content-restriction-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentRestrictionUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The restriction operation applied to content.\"\n    },\n    \"restrictions\": {\n      \"type\": \"object\",\n      \"description\": \"The users/groups that the restrictions will be applied to. At least one of\\n`user` or `group` must be specified for this object.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-restriction-update-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentRestrictionUpdate
---

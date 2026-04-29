---
description: Options for issue export.
layout: schema
name: export_options
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: project_key
  type: string
- description: ''
  name: project_name
  type: string
- description: ''
  name: send_email
  type: boolean
- description: ''
  name: include_attachments
  type: boolean
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-export_options-schema.json
slug: atlassian-bitbucket-repositories-export_options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"export_options\",\n  \"type\": \"object\",\n  \"description\": \"Options for issue export.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"project_key\": {\n      \"type\": \"string\"\n    },\n    \"project_name\": {\n      \"type\": \"string\"\n    },\n    \"send_email\": {\n      \"type\": \"boolean\"\n    },\n    \"include_attachments\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-export_options-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: export_options
---

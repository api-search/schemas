---
description: A Role defines a set of permissions for accessing workflows, lookups, reports, and support in Cflow.
layout: schema
name: Cflow Role
properties_list:
- description: Unique identifier of the role.
  name: id
  type: string
- description: Name of the role.
  name: name
  type: string
- description: Permission settings for this role across workflows, lookups, reports, and support.
  name: permissions
  type: object
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/role.json
slug: role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cflow/blob/main/json-schema/role.json\",\n  \"title\": \"Cflow Role\",\n  \"description\": \"A Role defines a set of permissions for accessing workflows, lookups, reports, and support in Cflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the role.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the role.\"\n    },\n    \"permissions\": {\n      \"type\": \"object\",\n      \"description\": \"Permission settings for this role across workflows, lookups, reports, and support.\",\n      \"properties\": {\n        \"workflows\": {\n          \"type\": \"string\",\n          \"description\": \"Permission level for workflows.\"\n        },\n        \"lookups\": {\n          \"type\": \"string\",\n          \"description\": \"Permission\
  \ level for lookups.\"\n        },\n        \"reports\": {\n          \"type\": \"string\",\n          \"description\": \"Permission level for reports.\"\n        },\n        \"support\": {\n          \"type\": \"string\",\n          \"description\": \"Permission level for support.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/json-schema/role.json
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Role
---

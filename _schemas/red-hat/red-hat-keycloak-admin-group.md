---
description: A group that enables bulk role and attribute assignment to users.
layout: schema
name: Group
properties_list:
- description: The unique identifier of the group.
  name: id
  type: string
- description: The name of the group.
  name: name
  type: string
- description: The full path of the group in the hierarchy.
  name: path
  type: string
- description: Child groups.
  name: subGroups
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-keycloak-admin-group-schema.json
slug: red-hat-keycloak-admin-group
source_filename: red-hat-keycloak-admin-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"description\": \"A group that enables bulk role and attribute assignment to users.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the group.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the group.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The full path of the group in the hierarchy.\"\n    },\n    \"subGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Child groups.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-keycloak-admin-group-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Group
---

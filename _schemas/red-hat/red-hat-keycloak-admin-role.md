---
description: A role that can be assigned to users or groups for authorization.
layout: schema
name: Role
properties_list:
- description: The unique identifier of the role.
  name: id
  type: string
- description: The name of the role.
  name: name
  type: string
- description: A description of the role.
  name: description
  type: string
- description: Whether this is a composite role containing other roles.
  name: composite
  type: boolean
- description: Whether this is a client-level role.
  name: clientRole
  type: boolean
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-keycloak-admin-role-schema.json
slug: red-hat-keycloak-admin-role
source_filename: red-hat-keycloak-admin-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Role\",\n  \"type\": \"object\",\n  \"description\": \"A role that can be assigned to users or groups for authorization.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the role.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the role.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the role.\"\n    },\n    \"composite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a composite role containing other roles.\"\n    },\n    \"clientRole\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a client-level role.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-keycloak-admin-role-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Role
---

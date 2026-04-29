---
description: A Quay user account.
layout: schema
name: User
properties_list:
- description: The username.
  name: username
  type: string
- description: The user's email address.
  name: email
  type: string
- description: Whether the user's email has been verified.
  name: verified
  type: boolean
- description: Organizations the user belongs to.
  name: organizations
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-user-schema.json
slug: red-hat-quay-user
source_filename: red-hat-quay-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A Quay user account.\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The user's email address.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user's email has been verified.\"\n    },\n    \"organizations\": {\n      \"type\": \"array\",\n      \"description\": \"Organizations the user belongs to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-user-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: User
---

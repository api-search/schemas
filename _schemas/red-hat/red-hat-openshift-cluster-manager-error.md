---
description: An error response from the API.
layout: schema
name: Error
properties_list:
- description: The error kind identifier.
  name: kind
  type: string
- description: The numeric error identifier.
  name: id
  type: string
- description: A link to the error documentation.
  name: href
  type: string
- description: The error code.
  name: code
  type: string
- description: A human-readable description of the error.
  name: reason
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-manager-error-schema.json
slug: red-hat-openshift-cluster-manager-error
source_filename: red-hat-openshift-cluster-manager-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"An error response from the API.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The error kind identifier.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The numeric error identifier.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"A link to the error documentation.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-manager-error-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Error
---

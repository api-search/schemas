---
description: Represents a textual expression in the Common Expression Language (CEL) syntax. Used for conditional access policies.
layout: schema
name: Expr
properties_list:
- description: 'The CEL expression string. Example: request.time < timestamp("2024-01-01T00:00:00Z").'
  name: expression
  type: string
- description: An optional title for the expression.
  name: title
  type: string
- description: An optional description of the expression.
  name: description
  type: string
- description: An optional string indicating the location of the expression for error reporting.
  name: location
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-expr-schema.json
slug: cloud-resource-manager-expr
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Expr\",\n  \"type\": \"object\",\n  \"description\": \"Represents a textual expression in the Common Expression Language (CEL) syntax. Used for conditional access policies.\",\n  \"properties\": {\n    \"expression\": {\n      \"type\": \"string\",\n      \"description\": \"The CEL expression string. Example: request.time < timestamp(\\\"2024-01-01T00:00:00Z\\\").\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"An optional title for the expression.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description of the expression.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"An optional string indicating the location of the expression for error reporting.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-expr-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: Expr
---

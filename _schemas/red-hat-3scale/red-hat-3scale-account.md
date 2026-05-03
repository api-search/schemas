---
description: Schema for a developer account in Red Hat 3scale API Management.
layout: schema
name: Red Hat 3scale Account
properties_list:
- description: Unique account identifier
  name: id
  type: integer
- description: Account creation timestamp
  name: created_at
  type: string
- description: Account last updated timestamp
  name: updated_at
  type: string
- description: Account approval state
  name: state
  type: string
- description: Organization name for the developer account
  name: org_name
  type: string
- description: Custom fields defined in the developer portal
  name: extra_fields
  type: object
provider_name: Red Hat 3scale
provider_slug: red-hat-3scale
schema_file: json-schema/red-hat-3scale-account-schema.json
slug: red-hat-3scale-account
source_filename: red-hat-3scale-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/red-hat-3scale/json-schema/red-hat-3scale-account-schema.json\",\n  \"title\": \"Red Hat 3scale Account\",\n  \"description\": \"Schema for a developer account in Red Hat 3scale API Management.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"state\", \"org_name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account creation timestamp\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account last updated timestamp\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"approved\", \"pending\", \"rejected\"],\n      \"description\": \"Account approval state\"\n    },\n \
  \   \"org_name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name for the developer account\",\n      \"minLength\": 1\n    },\n    \"extra_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom fields defined in the developer portal\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/json-schema/red-hat-3scale-account-schema.json
tags:
- API Gateway
- API Management
- Developer Portal
- Enterprise
- Red Hat
title: Red Hat 3scale Account
---

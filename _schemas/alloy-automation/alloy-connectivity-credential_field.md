---
description: A required field for credential creation
layout: schema
name: CredentialField
properties_list:
- description: Field name
  name: name
  type: string
- description: Field description
  name: description
  type: string
- description: Whether this field is required
  name: required
  type: boolean
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-credential_field-schema.json
slug: alloy-connectivity-credential_field
source_filename: alloy-connectivity-credential_field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-credential_field-schema.json\",\n  \"title\": \"CredentialField\",\n  \"type\": \"object\",\n  \"description\": \"A required field for credential creation\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Field name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Field description\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this field is required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-credential_field-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: CredentialField
---

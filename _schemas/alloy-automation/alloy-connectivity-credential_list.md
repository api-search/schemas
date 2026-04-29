---
description: List of credentials for a user on a connector
layout: schema
name: CredentialList
properties_list:
- description: List of credential records
  name: credentials
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-credential_list-schema.json
slug: alloy-connectivity-credential_list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-credential_list-schema.json\",\n  \"title\": \"CredentialList\",\n  \"type\": \"object\",\n  \"description\": \"List of credentials for a user on a connector\",\n  \"properties\": {\n    \"credentials\": {\n      \"type\": \"array\",\n      \"description\": \"List of credential records\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-credential_list-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: CredentialList
---

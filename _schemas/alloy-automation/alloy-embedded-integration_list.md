---
description: List of available integrations
layout: schema
name: IntegrationList
properties_list:
- description: List of integration records
  name: integrations
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-integration_list-schema.json
slug: alloy-embedded-integration_list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-integration_list-schema.json\",\n  \"title\": \"IntegrationList\",\n  \"type\": \"object\",\n  \"description\": \"List of available integrations\",\n  \"properties\": {\n    \"integrations\": {\n      \"type\": \"array\",\n      \"description\": \"List of integration records\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-integration_list-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: IntegrationList
---

---
description: List of available connectors
layout: schema
name: ConnectorList
properties_list:
- description: List of connector records
  name: connectors
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-connector_list-schema.json
slug: alloy-connectivity-connector_list
source_filename: alloy-connectivity-connector_list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-connector_list-schema.json\",\n  \"title\": \"ConnectorList\",\n  \"type\": \"object\",\n  \"description\": \"List of available connectors\",\n  \"properties\": {\n    \"connectors\": {\n      \"type\": \"array\",\n      \"description\": \"List of connector records\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-connector_list-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ConnectorList
---

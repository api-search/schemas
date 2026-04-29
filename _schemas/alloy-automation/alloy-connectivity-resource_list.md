---
description: List of resources for a connector
layout: schema
name: ResourceList
properties_list:
- description: List of resource records
  name: resources
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-resource_list-schema.json
slug: alloy-connectivity-resource_list
source_filename: alloy-connectivity-resource_list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-resource_list-schema.json\",\n  \"title\": \"ResourceList\",\n  \"type\": \"object\",\n  \"description\": \"List of resources for a connector\",\n  \"properties\": {\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of resource records\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-resource_list-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ResourceList
---

---
description: An embedded integration available in the Apifuse marketplace.
layout: schema
name: Integration
properties_list:
- description: Unique identifier of the integration.
  name: id
  type: string
- description: Display name of the integration.
  name: name
  type: string
- description: Category of the integration.
  name: category
  type: string
- description: Current status of the integration.
  name: status
  type: string
- description: Description of what the integration does.
  name: description
  type: string
provider_name: Apifuse
provider_slug: apifuse
schema_file: json-schema/apifuse-integration-schema.json
slug: apifuse-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"description\": \"An embedded integration available in the Apifuse marketplace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the integration.\",\n      \"example\": \"int-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the integration.\",\n      \"example\": \"Salesforce\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the integration.\",\n      \"example\": \"CRM\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"beta\"\n      ],\n      \"description\": \"Current status\
  \ of the integration.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the integration does.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-integration-schema.json
tags:
- Embedded Integrations
- Integration Platform
- Integrations
- iPaaS
- Marketplace
- SaaS
- Workflow Automation
title: Integration
---

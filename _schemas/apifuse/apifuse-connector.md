---
description: A pre-built connector for a specific platform in Apifuse.
layout: schema
name: Connector
properties_list:
- description: Unique identifier of the connector.
  name: id
  type: string
- description: Display name of the connector.
  name: name
  type: string
- description: Category of the connector.
  name: category
  type: string
- description: Authentication type used by this connector.
  name: authType
  type: string
provider_name: Apifuse
provider_slug: apifuse
schema_file: json-schema/apifuse-connector-schema.json
slug: apifuse-connector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-connector-schema.json\",\n  \"title\": \"Connector\",\n  \"description\": \"A pre-built connector for a specific platform in Apifuse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the connector.\",\n      \"example\": \"conn-salesforce\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the connector.\",\n      \"example\": \"Salesforce\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the connector.\",\n      \"example\": \"CRM\"\n    },\n    \"authType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"oauth2\",\n        \"apikey\",\n        \"basic\"\n      ],\n      \"description\": \"Authentication type\
  \ used by this connector.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-connector-schema.json
tags:
- Embedded Integrations
- Integration Platform
- Integrations
- iPaaS
- Marketplace
- SaaS
- Workflow Automation
title: Connector
---

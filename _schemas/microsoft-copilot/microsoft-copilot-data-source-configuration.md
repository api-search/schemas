---
description: Additional configuration for applicable data sources.
layout: schema
name: DataSourceConfiguration
properties_list:
- description: Configuration for Copilot connectors retrieval.
  name: externalItem
  type: object
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-data-source-configuration-schema.json
slug: microsoft-copilot-data-source-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Additional configuration for applicable data sources.\",\n  \"properties\": {\n    \"externalItem\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for Copilot connectors retrieval.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-data-source-configuration-schema.json
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
title: DataSourceConfiguration
---

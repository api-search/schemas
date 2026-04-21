---
description: Schema representing an AI model integrated with the APIPark AI gateway
layout: schema
name: APIPark AI Model
properties_list:
- description: Unique identifier of the AI model integration
  name: id
  type: string
- description: AI provider name (e.g., OpenAI, Anthropic, Gemini)
  name: provider
  type: string
- description: Name of the AI model
  name: modelName
  type: string
- description: ''
  name: status
  type: string
- description: Load balancing priority
  name: priority
  type: integer
provider_name: APIPark
provider_slug: apipark
schema_file: json-schema/apipark-ai-model-schema.json
slug: apipark-ai-model
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- LLM
- Open Source
title: APIPark AI Model
---

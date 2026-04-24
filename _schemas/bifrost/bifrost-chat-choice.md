---
description: A single completion choice in the response.
layout: schema
name: ChatChoice
properties_list:
- description: Index of this choice.
  name: index
  type: integer
- description: ''
  name: message
  type: object
- description: Reason the generation stopped.
  name: finish_reason
  type: string
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-choice-schema.json
slug: bifrost-chat-choice
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatChoice
---

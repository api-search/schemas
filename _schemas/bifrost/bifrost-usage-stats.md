---
description: Token usage statistics for the completion.
layout: schema
name: UsageStats
properties_list:
- description: Number of tokens in the prompt.
  name: prompt_tokens
  type: integer
- description: Number of tokens generated.
  name: completion_tokens
  type: integer
- description: Total tokens used.
  name: total_tokens
  type: integer
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-usage-stats-schema.json
slug: bifrost-usage-stats
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: UsageStats
---

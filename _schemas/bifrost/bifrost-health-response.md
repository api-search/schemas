---
description: Gateway health status response.
layout: schema
name: HealthResponse
properties_list:
- description: Overall gateway status.
  name: status
  type: string
- description: Gateway version.
  name: version
  type: string
- description: Status of configured providers.
  name: providers
  type: array
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-health-response-schema.json
slug: bifrost-health-response
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: HealthResponse
---

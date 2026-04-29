---
description: A Stream Route is used for Layer 4 (TCP/UDP) traffic proxying.
layout: schema
name: Apache APISIX Stream Route
properties_list:
- description: Description of the stream route.
  name: desc
  type: string
- description: Client IP address to match.
  name: remote_addr
  type: string
- description: Server address to match.
  name: server_addr
  type: string
- description: Server port to match.
  name: server_port
  type: integer
- description: Server Name Indication value to match.
  name: sni
  type: string
- description: Plugin configuration for the stream route.
  name: plugins
  type: object
- description: Inline upstream configuration.
  name: upstream
  type: object
- description: ID of an existing upstream to use.
  name: upstream_id
  type: string
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/stream-route.json
slug: stream-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/stream-route.json\",\n  \"title\": \"Apache APISIX Stream Route\",\n  \"description\": \"A Stream Route is used for Layer 4 (TCP/UDP) traffic proxying.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the stream route.\"\n    },\n    \"remote_addr\": {\n      \"type\": \"string\",\n      \"description\": \"Client IP address to match.\"\n    },\n    \"server_addr\": {\n      \"type\": \"string\",\n      \"description\": \"Server address to match.\"\n    },\n    \"server_port\": {\n      \"type\": \"integer\",\n      \"description\": \"Server port to match.\"\n    },\n    \"sni\": {\n      \"type\": \"string\",\n      \"description\": \"Server Name Indication value to match.\"\n    },\n    \"plugins\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Plugin configuration for the stream route.\"\n    },\n    \"upstream\": {\n      \"$ref\": \"upstream.json\",\n      \"description\": \"Inline upstream configuration.\"\n    },\n    \"upstream_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of an existing upstream to use.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/stream-route.json
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Stream Route
---

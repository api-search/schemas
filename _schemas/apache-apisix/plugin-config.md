---
description: A Plugin Config is a reusable set of plugin configurations that can be bound to routes.
layout: schema
name: Apache APISIX Plugin Config
properties_list:
- description: Description of the plugin config.
  name: desc
  type: string
- description: Plugin configuration.
  name: plugins
  type: object
- description: Key-value pairs for categorization.
  name: labels
  type: object
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/plugin-config.json
slug: plugin-config
source_filename: plugin-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/plugin-config.json\",\n  \"title\": \"Apache APISIX Plugin Config\",\n  \"description\": \"A Plugin Config is a reusable set of plugin configurations that can be bound to routes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the plugin config.\"\n    },\n    \"plugins\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin configuration.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/plugin-config.json
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Plugin Config
---

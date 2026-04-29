---
description: A Consumer Group is a set of plugins that can be applied to multiple consumers rather than configuring each consumer individually.
layout: schema
name: Apache APISIX Consumer Group
properties_list:
- description: Description of the consumer group.
  name: desc
  type: string
- description: Plugin configuration shared among consumers in this group.
  name: plugins
  type: object
- description: Key-value pairs for categorization.
  name: labels
  type: object
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/consumer-group.json
slug: consumer-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/consumer-group.json\",\n  \"title\": \"Apache APISIX Consumer Group\",\n  \"description\": \"A Consumer Group is a set of plugins that can be applied to multiple consumers rather than configuring each consumer individually.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the consumer group.\"\n    },\n    \"plugins\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin configuration shared among consumers in this group.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/consumer-group.json
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Consumer Group
---

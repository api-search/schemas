---
description: A Consumer is an entity that consumes API services and is identified by a username.
layout: schema
name: Apache APISIX Consumer
properties_list:
- description: Unique username for the consumer.
  name: username
  type: string
- description: Description of the consumer.
  name: desc
  type: string
- description: Plugin configuration bound to this consumer.
  name: plugins
  type: object
- description: Key-value pairs for categorization.
  name: labels
  type: object
- description: ID of a consumer group this consumer belongs to.
  name: group_id
  type: string
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/consumer.json
slug: consumer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/consumer.json\",\n  \"title\": \"Apache APISIX Consumer\",\n  \"description\": \"A Consumer is an entity that consumes API services and is identified by a username.\",\n  \"type\": \"object\",\n  \"required\": [\"username\"],\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Unique username for the consumer.\"\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the consumer.\"\n    },\n    \"plugins\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin configuration bound to this consumer.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    },\n    \"group_id\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"ID of a consumer group this consumer belongs to.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/consumer.json
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Consumer
---

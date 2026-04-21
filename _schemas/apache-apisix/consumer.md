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

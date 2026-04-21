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

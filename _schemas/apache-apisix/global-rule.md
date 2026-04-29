---
description: A Global Rule applies plugin configurations to all requests processed by the APISIX instance.
layout: schema
name: Apache APISIX Global Rule
properties_list:
- description: Plugin configuration to apply globally.
  name: plugins
  type: object
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/global-rule.json
slug: global-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/global-rule.json\",\n  \"title\": \"Apache APISIX Global Rule\",\n  \"description\": \"A Global Rule applies plugin configurations to all requests processed by the APISIX instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plugins\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin configuration to apply globally.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/global-rule.json
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Global Rule
---

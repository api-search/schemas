---
description: List of Camel routes
layout: schema
name: RouteList
properties_list:
- description: ''
  name: routes
  type: array
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-route-list-schema.json
slug: apache-servicemix-route-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-route-list-schema.json\",\n  \"title\": \"RouteList\",\n  \"description\": \"List of Camel routes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Route\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-route-list-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: RouteList
---

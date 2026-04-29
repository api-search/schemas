---
description: List of web service endpoints
layout: schema
name: EndpointList
properties_list:
- description: ''
  name: endpoints
  type: array
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-endpoint-list-schema.json
slug: apache-servicemix-endpoint-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-endpoint-list-schema.json\",\n  \"title\": \"EndpointList\",\n  \"description\": \"List of web service endpoints\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Endpoint\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-endpoint-list-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: EndpointList
---

---
description: Response for listing namespaces.
layout: schema
name: ListNamespacesResponse
properties_list:
- description: ''
  name: Namespaces
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-list-namespaces-response-schema.json
slug: cloud-map-list-namespaces-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-list-namespaces-response-schema.json\",\n  \"title\": \"ListNamespacesResponse\",\n  \"description\": \"Response for listing namespaces.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Namespaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Namespace\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-list-namespaces-response-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: ListNamespacesResponse
---

---
description: Response for listing services.
layout: schema
name: ListServicesResponse
properties_list:
- description: ''
  name: Services
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Cloud Map
provider_slug: amazon-cloud-map
schema_file: json-schema/cloud-map-list-services-response-schema.json
slug: cloud-map-list-services-response
source_filename: cloud-map-list-services-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-list-services-response-schema.json\",\n  \"title\": \"ListServicesResponse\",\n  \"description\": \"Response for listing services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Service\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud-map/refs/heads/main/json-schema/cloud-map-list-services-response-schema.json
tags:
- AWS
- Cloud Map
- Service Discovery
- Microservices
- DNS
title: ListServicesResponse
---

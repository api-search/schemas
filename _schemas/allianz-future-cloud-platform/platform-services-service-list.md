---
description: Paginated list of platform services
layout: schema
name: ServiceList
properties_list:
- description: Total number of registered services
  name: total
  type: integer
- description: List of service records
  name: items
  type: array
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-service-list-schema.json
slug: platform-services-service-list
source_filename: platform-services-service-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-service-list-schema.json\",\n  \"title\": \"ServiceList\",\n  \"description\": \"Paginated list of platform services\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of registered services\",\n      \"example\": 62\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of service records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Service\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-service-list-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: ServiceList
---

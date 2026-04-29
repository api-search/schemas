---
description: List of platform namespaces
layout: schema
name: NamespaceList
properties_list:
- description: Total number of namespaces
  name: total
  type: integer
- description: List of namespace records
  name: items
  type: array
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-namespace-list-schema.json
slug: platform-services-namespace-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-namespace-list-schema.json\",\n  \"title\": \"NamespaceList\",\n  \"description\": \"List of platform namespaces\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of namespaces\",\n      \"example\": 12\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of namespace records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Namespace\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-namespace-list-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: NamespaceList
---

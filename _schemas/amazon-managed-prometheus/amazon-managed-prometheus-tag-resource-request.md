---
description: TagResourceRequest schema from Amazon Managed Service for Prometheus API
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-tag-resource-request-schema.json
slug: amazon-managed-prometheus-tag-resource-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon Managed Service for Prometheus API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"$ref\": \"#/components/schemas/TagMap\"\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-tag-resource-request-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: TagResourceRequest
---

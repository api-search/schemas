---
description: A Kubernetes namespace managed on the platform
layout: schema
name: Namespace
properties_list:
- description: Unique identifier for the namespace
  name: namespace_id
  type: string
- description: Kubernetes namespace name
  name: name
  type: string
- description: Team owning this namespace
  name: team
  type: string
- description: Number of services in this namespace
  name: service_count
  type: integer
- description: Namespace status
  name: status
  type: string
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-namespace-schema.json
slug: platform-services-namespace
source_filename: platform-services-namespace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-namespace-schema.json\",\n  \"title\": \"Namespace\",\n  \"description\": \"A Kubernetes namespace managed on the platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the namespace\",\n      \"example\": \"ns-500111\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace name\",\n      \"example\": \"insurance-policy\"\n    },\n    \"team\": {\n      \"type\": \"string\",\n      \"description\": \"Team owning this namespace\",\n      \"example\": \"policy-team\"\n    },\n    \"service_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of services in this namespace\",\n      \"example\": 8\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace status\",\n      \"enum\": [\n        \"active\",\n        \"provisioning\",\n        \"decommissioning\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-namespace-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: Namespace
---

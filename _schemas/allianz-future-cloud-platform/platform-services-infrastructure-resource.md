---
description: A provisioned cloud infrastructure resource
layout: schema
name: InfrastructureResource
properties_list:
- description: Unique identifier for the resource
  name: resource_id
  type: string
- description: Type of infrastructure resource
  name: resource_type
  type: string
- description: Resource name
  name: name
  type: string
- description: Associated Kubernetes namespace
  name: namespace
  type: string
- description: Provisioning status
  name: status
  type: string
- description: Timestamp when provisioning was initiated
  name: created_at
  type: string
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-infrastructure-resource-schema.json
slug: platform-services-infrastructure-resource
source_filename: platform-services-infrastructure-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-infrastructure-resource-schema.json\",\n  \"title\": \"InfrastructureResource\",\n  \"description\": \"A provisioned cloud infrastructure resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the resource\",\n      \"example\": \"infra-500222\"\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of infrastructure resource\",\n      \"example\": \"redis\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name\",\n      \"example\": \"policy-cache\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Associated Kubernetes namespace\",\n      \"example\": \"\
  insurance-policy\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Provisioning status\",\n      \"enum\": [\n        \"provisioning\",\n        \"ready\",\n        \"failed\",\n        \"decommissioned\"\n      ],\n      \"example\": \"provisioning\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when provisioning was initiated\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-infrastructure-resource-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: InfrastructureResource
---

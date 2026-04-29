---
description: Resource allocation with assigned and reassigned counts
layout: schema
name: ResourceAllocation
properties_list:
- description: Number of resources assigned to this organization
  name: assigned
  type: number
- description: Number of resources reassigned to sub-organizations
  name: reassigned
  type: number
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-resource-allocation-schema.json
slug: mulesoft-anypoint-platform-resource-allocation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceAllocation\",\n  \"type\": \"object\",\n  \"description\": \"Resource allocation with assigned and reassigned counts\",\n  \"properties\": {\n    \"assigned\": {\n      \"type\": \"number\",\n      \"description\": \"Number of resources assigned to this organization\"\n    },\n    \"reassigned\": {\n      \"type\": \"number\",\n      \"description\": \"Number of resources reassigned to sub-organizations\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-resource-allocation-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: ResourceAllocation
---

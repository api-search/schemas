---
description: Identity for the resource.
layout: schema
name: Identity
properties_list:
- description: ''
  name: principalId
  type: string
- description: ''
  name: tenantId
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: userAssignedIdentities
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-identity-schema.json
slug: azure-cognitive-services-identity
source_filename: azure-cognitive-services-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Identity\",\n  \"type\": \"object\",\n  \"description\": \"Identity for the resource.\",\n  \"properties\": {\n    \"principalId\": {\n      \"type\": \"string\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"userAssignedIdentities\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-identity-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Identity
---

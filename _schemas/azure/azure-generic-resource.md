---
description: Resource information.
layout: schema
name: GenericResource
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: kind
  type: string
- description: ''
  name: managedBy
  type: string
- description: ''
  name: sku
  type: object
provider_name: Microsoft Azure
provider_slug: azure
schema_file: json-schema/azure-generic-resource-schema.json
slug: azure-generic-resource
source_filename: azure-generic-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/json-schema/azure-generic-resource-schema.json\",\n  \"title\": \"GenericResource\",\n  \"description\": \"Resource information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"managedBy\": {\n      \"type\": \"string\"\n    },\n    \"sku\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"tier\": {\n          \"type\":\
  \ \"string\"\n        },\n        \"capacity\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/json-schema/azure-generic-resource-schema.json
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Platform as a Service
- Storage
title: GenericResource
---

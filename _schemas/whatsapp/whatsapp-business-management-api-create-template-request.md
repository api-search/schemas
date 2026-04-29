---
description: CreateTemplateRequest from WhatsApp API
layout: schema
name: CreateTemplateRequest
properties_list:
- description: Template name (lowercase, underscores only, max 512 chars)
  name: name
  type: string
- description: Language code
  name: language
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: components
  type: array
- description: ''
  name: parameter_format
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-create-template-request-schema.json
slug: whatsapp-business-management-api-create-template-request
source_filename: whatsapp-business-management-api-create-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-create-template-request-schema.json\",\n  \"title\": \"CreateTemplateRequest\",\n  \"description\": \"CreateTemplateRequest from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name (lowercase, underscores only, max 512 chars)\",\n      \"maxLength\": 512,\n      \"pattern\": \"^[a-z][a-z0-9_]*$\",\n      \"example\": \"Example Business\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code\",\n      \"example\": \"en_US\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AUTHENTICATION\",\n        \"MARKETING\",\n        \"UTILITY\"\n      ],\n      \"example\": \"AUTHENTICATION\"\n    },\n    \"components\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TemplateComponentDefinition\"\n      }\n    },\n    \"parameter_format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POSITIONAL\",\n        \"NAMED\"\n      ],\n      \"example\": \"POSITIONAL\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"language\",\n    \"category\",\n    \"components\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-create-template-request-schema.json
tags: []
title: CreateTemplateRequest
---

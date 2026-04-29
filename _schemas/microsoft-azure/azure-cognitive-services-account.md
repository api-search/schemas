---
description: Cognitive Services account.
layout: schema
name: Account
properties_list:
- description: Fully qualified resource ID.
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: Resource ETag.
  name: etag
  type: string
- description: The kind (type) of cognitive service account. Examples include OpenAI, TextAnalytics, ComputerVision, SpeechServices, etc.
  name: kind
  type: string
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: Resource tags.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-account-schema.json
slug: azure-cognitive-services-account
source_filename: azure-cognitive-services-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"Cognitive Services account.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Resource ETag.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind (type) of cognitive service account. Examples include OpenAI, TextAnalytics, ComputerVision, SpeechServices, etc.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Resource tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-account-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Account
---

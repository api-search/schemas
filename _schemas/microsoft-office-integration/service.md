---
description: A subscribed Office 365 service as returned by the Service Communications API.
layout: schema
name: Service
properties_list:
- description: The service identifier (e.g. Exchange, Lync, SharePoint).
  name: Id
  type: string
- description: The display name of the service.
  name: DisplayName
  type: string
- description: List of feature names available for the service.
  name: FeatureNames
  type: array
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
schema_file: json-schema/service.json
slug: service
source_filename: service.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"service.json\",\n  \"title\": \"Service\",\n  \"description\": \"A subscribed Office 365 service as returned by the Service Communications API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The service identifier (e.g. Exchange, Lync, SharePoint).\"\n    },\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the service.\"\n    },\n    \"FeatureNames\": {\n      \"type\": \"array\",\n      \"description\": \"List of feature names available for the service.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"Id\", \"DisplayName\", \"FeatureNames\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/json-schema/service.json
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
title: Service
---

---
description: OData collection response containing contact records.
layout: schema
name: ContactCollection
properties_list:
- description: OData context URL describing the collection.
  name: '@odata.context'
  type: string
- description: Total count of matching records (when $count=true).
  name: '@odata.count'
  type: integer
- description: URL to retrieve the next page of results.
  name: '@odata.nextLink'
  type: string
- description: Array of contact records.
  name: value
  type: array
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
schema_file: json-schema/microsoft-power-apps-dataverse-web-contact-collection-schema.json
slug: microsoft-power-apps-dataverse-web-contact-collection
source_filename: microsoft-power-apps-dataverse-web-contact-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactCollection\",\n  \"type\": \"object\",\n  \"description\": \"OData collection response containing contact records.\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\",\n      \"description\": \"OData context URL describing the collection.\"\n    },\n    \"@odata.count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total count of matching records (when $count=true).\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"URL to retrieve the next page of results.\"\n    },\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of contact records.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/json-schema/microsoft-power-apps-dataverse-web-contact-collection-schema.json
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
title: ContactCollection
---

---
description: ''
layout: schema
name: UserCollectionResponse
properties_list:
- description: The OData context URL for the collection.
  name: '@odata.context'
  type: string
- description: The total count of items in the collection (if requested).
  name: '@odata.count'
  type: integer
- description: The URL to retrieve the next page of results.
  name: '@odata.nextLink'
  type: string
- description: ''
  name: value
  type: array
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-user-collection-response-schema.json
slug: microsoft-graph-user-collection-response
source_filename: microsoft-graph-user-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCollectionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\",\n      \"description\": \"The OData context URL for the collection.\"\n    },\n    \"@odata.count\": {\n      \"type\": \"integer\",\n      \"description\": \"The total count of items in the collection (if requested).\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to retrieve the next page of results.\"\n    },\n    \"value\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-user-collection-response-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: UserCollectionResponse
---

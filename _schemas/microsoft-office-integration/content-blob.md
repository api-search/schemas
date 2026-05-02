---
description: A content blob reference from the Office 365 Management Activity API representing aggregated audit actions and events available for retrieval.
layout: schema
name: ContentBlob
properties_list:
- description: The content type of the blob.
  name: contentType
  type: string
- description: An opaque string that uniquely identifies the content.
  name: contentId
  type: string
- description: The URL to use when retrieving the content.
  name: contentUri
  type: string
- description: The datetime when the content was made available.
  name: contentCreated
  type: string
- description: The datetime after which the content will no longer be available for retrieval.
  name: contentExpiration
  type: string
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
schema_file: json-schema/content-blob.json
slug: content-blob
source_filename: content-blob.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"content-blob.json\",\n  \"title\": \"ContentBlob\",\n  \"description\": \"A content blob reference from the Office 365 Management Activity API representing aggregated audit actions and events available for retrieval.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the blob.\",\n      \"enum\": [\n        \"Audit.AzureActiveDirectory\",\n        \"Audit.Exchange\",\n        \"Audit.SharePoint\",\n        \"Audit.General\",\n        \"DLP.All\"\n      ]\n    },\n    \"contentId\": {\n      \"type\": \"string\",\n      \"description\": \"An opaque string that uniquely identifies the content.\"\n    },\n    \"contentUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to use when retrieving the content.\"\n    },\n    \"contentCreated\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The datetime when the content was made available.\"\n    },\n    \"contentExpiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The datetime after which the content will no longer be available for retrieval.\"\n    }\n  },\n  \"required\": [\"contentType\", \"contentId\", \"contentUri\", \"contentCreated\", \"contentExpiration\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/json-schema/content-blob.json
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
title: ContentBlob
---

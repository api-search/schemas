---
description: Response message for listing folders.
layout: schema
name: ListFoldersResponse
properties_list:
- description: The list of folders under the specified parent.
  name: folders
  type: array
- description: Pagination token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-list-folders-response-schema.json
slug: cloud-resource-manager-list-folders-response
source_filename: cloud-resource-manager-list-folders-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListFoldersResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for listing folders.\",\n  \"properties\": {\n    \"folders\": {\n      \"type\": \"array\",\n      \"description\": \"The list of folders under the specified parent.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-list-folders-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: ListFoldersResponse
---

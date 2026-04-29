---
description: Response message for searching folders.
layout: schema
name: SearchFoldersResponse
properties_list:
- description: The list of folders matching the search criteria.
  name: folders
  type: array
- description: Pagination token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-search-folders-response-schema.json
slug: cloud-resource-manager-search-folders-response
source_filename: cloud-resource-manager-search-folders-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchFoldersResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for searching folders.\",\n  \"properties\": {\n    \"folders\": {\n      \"type\": \"array\",\n      \"description\": \"The list of folders matching the search criteria.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-search-folders-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: SearchFoldersResponse
---

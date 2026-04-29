---
description: Response message for listing tag values.
layout: schema
name: ListTagValuesResponse
properties_list:
- description: The list of tag values.
  name: tagValues
  type: array
- description: Pagination token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-list-tag-values-response-schema.json
slug: cloud-resource-manager-list-tag-values-response
source_filename: cloud-resource-manager-list-tag-values-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagValuesResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for listing tag values.\",\n  \"properties\": {\n    \"tagValues\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tag values.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-list-tag-values-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: ListTagValuesResponse
---

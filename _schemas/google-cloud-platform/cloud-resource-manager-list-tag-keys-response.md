---
description: Response message for listing tag keys.
layout: schema
name: ListTagKeysResponse
properties_list:
- description: The list of tag keys.
  name: tagKeys
  type: array
- description: Pagination token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-list-tag-keys-response-schema.json
slug: cloud-resource-manager-list-tag-keys-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagKeysResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for listing tag keys.\",\n  \"properties\": {\n    \"tagKeys\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tag keys.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-list-tag-keys-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: ListTagKeysResponse
---

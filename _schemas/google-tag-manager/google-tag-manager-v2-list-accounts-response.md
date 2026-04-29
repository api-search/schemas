---
description: List Accounts Response.
layout: schema
name: ListAccountsResponse
properties_list:
- description: List of GTM Accounts that a user has access to.
  name: account
  type: array
- description: Continuation token for fetching the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-list-accounts-response-schema.json
slug: google-tag-manager-v2-list-accounts-response
source_filename: google-tag-manager-v2-list-accounts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListAccountsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List Accounts Response.\",\n  \"properties\": {\n    \"account\": {\n      \"type\": \"array\",\n      \"description\": \"List of GTM Accounts that a user has access to.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Continuation token for fetching the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-list-accounts-response-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ListAccountsResponse
---

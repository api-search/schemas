---
description: Campaign list response.
layout: schema
name: CampaignsListResponse
properties_list:
- description: ''
  name: campaigns
  type: array
- description: Pagination token to be used in a subsequent request to retrieve the next page.
  name: nextPageToken
  type: string
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-campaigns-list-response-schema.json
slug: google-campaign-manager-campaigns-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CampaignsListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Campaign list response.\",\n  \"properties\": {\n    \"campaigns\": {\n      \"type\": \"array\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token to be used in a subsequent request to retrieve the next page.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-campaigns-list-response-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: CampaignsListResponse
---

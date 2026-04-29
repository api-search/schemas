---
description: Response message for searching organizations.
layout: schema
name: SearchOrganizationsResponse
properties_list:
- description: The list of organizations matching the search criteria.
  name: organizations
  type: array
- description: Pagination token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-search-organizations-response-schema.json
slug: cloud-resource-manager-search-organizations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchOrganizationsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for searching organizations.\",\n  \"properties\": {\n    \"organizations\": {\n      \"type\": \"array\",\n      \"description\": \"The list of organizations matching the search criteria.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-search-organizations-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: SearchOrganizationsResponse
---

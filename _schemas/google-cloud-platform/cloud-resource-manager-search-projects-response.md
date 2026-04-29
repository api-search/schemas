---
description: Response message for searching projects.
layout: schema
name: SearchProjectsResponse
properties_list:
- description: The list of projects matching the search criteria.
  name: projects
  type: array
- description: Pagination token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-search-projects-response-schema.json
slug: cloud-resource-manager-search-projects-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchProjectsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for searching projects.\",\n  \"properties\": {\n    \"projects\": {\n      \"type\": \"array\",\n      \"description\": \"The list of projects matching the search criteria.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-search-projects-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: SearchProjectsResponse
---

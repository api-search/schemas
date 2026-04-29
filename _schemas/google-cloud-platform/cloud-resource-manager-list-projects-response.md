---
description: Response message for listing projects.
layout: schema
name: ListProjectsResponse
properties_list:
- description: The list of projects under the specified parent.
  name: projects
  type: array
- description: Pagination token to retrieve the next page of results. Empty if there are no more results.
  name: nextPageToken
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-list-projects-response-schema.json
slug: cloud-resource-manager-list-projects-response
source_filename: cloud-resource-manager-list-projects-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListProjectsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message for listing projects.\",\n  \"properties\": {\n    \"projects\": {\n      \"type\": \"array\",\n      \"description\": \"The list of projects under the specified parent.\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token to retrieve the next page of results. Empty if there are no more results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-list-projects-response-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: ListProjectsResponse
---

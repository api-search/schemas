---
description: ListResponsePlansInput schema
layout: schema
name: ListResponsePlansInput
properties_list:
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-response-plans-input-schema.json
slug: incident-manager-list-response-plans-input
source_filename: incident-manager-list-response-plans-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-response-plans-input-schema.json\",\n  \"title\": \"ListResponsePlansInput\",\n  \"description\": \"ListResponsePlansInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of response plans per page.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-response-plans-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ListResponsePlansInput
---

---
description: BatchOrganizationResponse from LinkedIn API
layout: schema
name: BatchOrganizationResponse
properties_list:
- description: ''
  name: results
  type: object
- description: ''
  name: statuses
  type: object
- description: ''
  name: errors
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-batch-organization-response-schema.json
slug: linkedin-regulations-data-portability-batch-organization-response
source_filename: linkedin-regulations-data-portability-batch-organization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-batch-organization-response-schema.json\",\n  \"title\": \"BatchOrganizationResponse\",\n  \"description\": \"BatchOrganizationResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/OrganizationResponse\"\n      }\n    },\n    \"statuses\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/ErrorDetail\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-batch-organization-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: BatchOrganizationResponse
---

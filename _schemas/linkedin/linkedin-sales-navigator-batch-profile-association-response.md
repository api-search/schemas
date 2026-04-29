---
description: BatchProfileAssociationResponse from LinkedIn API
layout: schema
name: BatchProfileAssociationResponse
properties_list:
- description: ''
  name: statuses
  type: object
- description: ''
  name: results
  type: object
- description: ''
  name: errors
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-batch-profile-association-response-schema.json
slug: linkedin-sales-navigator-batch-profile-association-response
source_filename: linkedin-sales-navigator-batch-profile-association-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-batch-profile-association-response-schema.json\",\n  \"title\": \"BatchProfileAssociationResponse\",\n  \"description\": \"BatchProfileAssociationResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statuses\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"results\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/SalesNavigatorProfileAssociation\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-batch-profile-association-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: BatchProfileAssociationResponse
---

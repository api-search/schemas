---
description: ErrorResponse from LinkedIn API
layout: schema
name: ErrorResponse
properties_list:
- description: HTTP status code
  name: status
  type: integer
- description: Error message
  name: message
  type: string
- description: LinkedIn service-specific error code
  name: serviceErrorCode
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-learning-parent-application-error-response-schema.json
slug: linkedin-talent-learning-parent-application-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"ErrorResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\",\n      \"example\": 400\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"Invalid request parameters\"\n    },\n    \"serviceErrorCode\": {\n      \"type\": \"integer\",\n      \"description\": \"LinkedIn service-specific error code\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-error-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ErrorResponse
---

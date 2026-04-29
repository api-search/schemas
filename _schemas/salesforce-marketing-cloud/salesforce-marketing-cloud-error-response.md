---
description: Standard error response returned by the Marketing Cloud API
layout: schema
name: ErrorResponse
properties_list:
- description: Human-readable error message
  name: message
  type: string
- description: Numeric error code
  name: errorcode
  type: integer
- description: URL to relevant documentation for this error
  name: documentation
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-error-response-schema.json
slug: salesforce-marketing-cloud-error-response
source_filename: salesforce-marketing-cloud-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response returned by the Marketing Cloud API\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    },\n    \"errorcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric error code\"\n    },\n    \"documentation\": {\n      \"type\": \"string\",\n      \"description\": \"URL to relevant documentation for this error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-error-response-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: ErrorResponse
---

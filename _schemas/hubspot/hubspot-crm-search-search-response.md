---
description: The response from a CRM search operation.
layout: schema
name: SearchResponse
properties_list:
- description: The total number of records matching the search criteria.
  name: total
  type: integer
- description: The matching CRM records for the current page.
  name: results
  type: array
- description: Pagination information for the response.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-search-search-response-schema.json
slug: hubspot-crm-search-search-response
source_filename: hubspot-crm-search-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The response from a CRM search operation.\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of records matching the search criteria.\",\n      \"example\": 10\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The matching CRM records for the current page.\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A CRM object record returned from a search.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the CRM record.\",\n \
  \           \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The CRM record's properties as key-value pairs.\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the record was created.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the record was last updated.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the record has been archived.\",\n            \"example\": true\n          }\n        }\n      }\n    },\n    \"paging\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for the response.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Information for retrieving the next page of results.\",\n          \"example\": {\n            \"after\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"The cursor token to use in the after parameter for the next page.\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"A URL link to the next page of results.\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-search-search-response-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: SearchResponse
---

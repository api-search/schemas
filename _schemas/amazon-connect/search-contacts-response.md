---
description: SearchContactsResponse schema from Amazon Connect Service API
layout: schema
name: SearchContactsResponse
properties_list:
- description: ''
  name: Contacts
  type: array
- description: ''
  name: NextToken
  type: string
- description: The total count of the search result.
  name: TotalCount
  type: integer
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/search-contacts-response-schema.json
slug: search-contacts-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/search-contacts-response-schema.json\",\n  \"title\": \"SearchContactsResponse\",\n  \"description\": \"SearchContactsResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Contacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ContactSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"TotalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total count of the search result.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/search-contacts-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: SearchContactsResponse
---

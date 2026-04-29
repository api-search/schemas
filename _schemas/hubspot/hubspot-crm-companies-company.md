---
description: A HubSpot company record.
layout: schema
name: Company
properties_list:
- description: The unique identifier for the company.
  name: id
  type: string
- description: The company's properties as key-value pairs.
  name: properties
  type: object
- description: The date and time the company was created.
  name: createdAt
  type: string
- description: The date and time the company was last updated.
  name: updatedAt
  type: string
- description: Whether the company has been archived.
  name: archived
  type: boolean
- description: The company's associations with other CRM objects.
  name: associations
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-companies-company-schema.json
slug: hubspot-crm-companies-company
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A HubSpot company record.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the company.\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The company's properties as key-value pairs.\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the company was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the company was last updated.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company has been archived.\",\n\
  \      \"example\": true\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"description\": \"The company's associations with other CRM objects.\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Company\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-companies-company-schema.json
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
title: Company
---

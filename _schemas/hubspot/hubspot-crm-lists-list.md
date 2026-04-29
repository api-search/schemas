---
description: A HubSpot CRM list.
layout: schema
name: List
properties_list:
- description: The unique identifier for the list.
  name: listId
  type: string
- description: The name of the list.
  name: name
  type: string
- description: Whether the list is static (manually managed) or dynamic (filter-based).
  name: listType
  type: string
- description: The object type the list contains (e.g., 0-1 for contacts).
  name: objectTypeId
  type: string
- description: The current processing status of the list.
  name: processingStatus
  type: string
- description: The date and time the list was created.
  name: createdAt
  type: string
- description: The date and time the list was last updated.
  name: updatedAt
  type: string
- description: The filter definition for dynamic lists.
  name: filterBranch
  type: object
- description: The current number of members in the list.
  name: memberCount
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-lists-list-schema.json
slug: hubspot-crm-lists-list
source_filename: hubspot-crm-lists-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A HubSpot CRM list.\",\n  \"properties\": {\n    \"listId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the list.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the list.\",\n      \"example\": \"Example Record\"\n    },\n    \"listType\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the list is static (manually managed) or dynamic (filter-based).\",\n      \"example\": \"STATIC\",\n      \"enum\": [\n        \"STATIC\",\n        \"DYNAMIC\"\n      ]\n    },\n    \"objectTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"The object type the list contains (e.g., 0-1 for contacts).\",\n      \"example\": \"500123\"\n    },\n    \"processingStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status of the list.\",\n      \"example\": \"active\"\
  \n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the list was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the list was last updated.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"filterBranch\": {\n      \"type\": \"object\",\n      \"description\": \"The filter definition for dynamic lists.\",\n      \"example\": {}\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The current number of members in the list.\",\n      \"example\": 10\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"List\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-lists-list-schema.json
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
title: List
---

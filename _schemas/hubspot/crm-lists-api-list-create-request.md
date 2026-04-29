---
description: Request body for creating a new CRM list.
layout: schema
name: ListCreateRequest
properties_list:
- description: The name of the list.
  name: name
  type: string
- description: The object type ID for the list (e.g., 0-1 for contacts).
  name: objectTypeId
  type: string
- description: The type of list processing.
  name: processingType
  type: string
- description: The filter branch definition for dynamic lists.
  name: filterBranch
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-lists-api-list-create-request-schema.json
slug: crm-lists-api-list-create-request
source_filename: crm-lists-api-list-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-lists-api-list-create-request-schema.json\",\n  \"title\": \"ListCreateRequest\",\n  \"description\": \"Request body for creating a new CRM list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the list.\",\n      \"example\": \"Example Record\"\n    },\n    \"objectTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"The object type ID for the list (e.g., 0-1 for contacts).\",\n      \"example\": \"500123\"\n    },\n    \"processingType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MANUAL\",\n        \"DYNAMIC\",\n        \"SNAPSHOT\"\n      ],\n      \"description\": \"The type of list processing.\",\n      \"example\": \"MANUAL\"\n    },\n    \"filterBranch\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"The filter branch definition for dynamic lists.\",\n      \"example\": {}\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"objectTypeId\",\n    \"processingType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-lists-api-list-create-request-schema.json
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
title: ListCreateRequest
---

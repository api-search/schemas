---
description: A CRM object record returned from a search.
layout: schema
name: CRMObject
properties_list:
- description: The unique identifier for the CRM record.
  name: id
  type: string
- description: The CRM record's properties as key-value pairs.
  name: properties
  type: object
- description: The date and time the record was created.
  name: createdAt
  type: string
- description: The date and time the record was last updated.
  name: updatedAt
  type: string
- description: Whether the record has been archived.
  name: archived
  type: boolean
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-search-api-crmobject-schema.json
slug: crm-search-api-crmobject
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-crmobject-schema.json\",\n  \"title\": \"CRMObject\",\n  \"description\": \"A CRM object record returned from a search.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the CRM record.\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The CRM record's properties as key-value pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n \
  \   \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last updated.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record has been archived.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-crmobject-schema.json
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
title: CRMObject
---

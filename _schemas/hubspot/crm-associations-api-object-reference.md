---
description: Reference to a CRM object by ID
layout: schema
name: ObjectReference
properties_list:
- description: ID of the object
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-object-reference-schema.json
slug: crm-associations-api-object-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-object-reference-schema.json\",\n  \"title\": \"ObjectReference\",\n  \"description\": \"Reference to a CRM object by ID\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the object\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-object-reference-schema.json
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
title: ObjectReference
---

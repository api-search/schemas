---
description: Defines the type of association
layout: schema
name: AssociationType
properties_list:
- description: Category of the association type
  name: associationCategory
  type: string
- description: Numeric identifier for the association type
  name: associationTypeId
  type: integer
- description: Human-readable label for the association
  name: label
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-association-type-schema.json
slug: crm-associations-api-association-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-association-type-schema.json\",\n  \"title\": \"AssociationType\",\n  \"description\": \"Defines the type of association\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associationCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ],\n      \"description\": \"Category of the association type\",\n      \"example\": \"HUBSPOT_DEFINED\"\n    },\n    \"associationTypeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the association type\",\n      \"example\": 500123\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the association\",\n      \"example\": \"Example Record\"\n    }\n  },\n  \"\
  required\": [\n    \"associationCategory\",\n    \"associationTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-association-type-schema.json
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
title: AssociationType
---

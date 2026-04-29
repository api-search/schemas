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
schema_file: json-schema/hubspot-crm-associations-association-type-schema.json
slug: hubspot-crm-associations-association-type
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Defines the type of association\",\n  \"properties\": {\n    \"associationCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the association type\",\n      \"example\": \"HUBSPOT_DEFINED\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ]\n    },\n    \"associationTypeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the association type\",\n      \"example\": 500123\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the association\",\n      \"example\": \"Example Record\"\n    }\n  },\n  \"required\": [\n    \"associationCategory\",\n    \"associationTypeId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-association-type-schema.json
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

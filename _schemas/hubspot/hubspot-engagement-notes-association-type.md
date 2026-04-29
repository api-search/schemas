---
description: Type of association
layout: schema
name: AssociationType
properties_list:
- description: The category of association
  name: associationCategory
  type: string
- description: The association type ID
  name: associationTypeId
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-association-type-schema.json
slug: hubspot-engagement-notes-association-type
source_filename: hubspot-engagement-notes-association-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Type of association\",\n  \"properties\": {\n    \"associationCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of association\",\n      \"example\": \"HUBSPOT_DEFINED\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ]\n    },\n    \"associationTypeId\": {\n      \"type\": \"integer\",\n      \"description\": \"The association type ID\",\n      \"example\": 202\n    }\n  },\n  \"required\": [\n    \"associationCategory\",\n    \"associationTypeId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-association-type-schema.json
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

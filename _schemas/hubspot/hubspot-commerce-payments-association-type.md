---
description: An association type definition
layout: schema
name: AssociationType
properties_list:
- description: The category of the association
  name: associationCategory
  type: string
- description: The numeric ID of the association type
  name: associationTypeId
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-association-type-schema.json
slug: hubspot-commerce-payments-association-type
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An association type definition\",\n  \"properties\": {\n    \"associationCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the association\",\n      \"example\": \"HUBSPOT_DEFINED\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ]\n    },\n    \"associationTypeId\": {\n      \"type\": \"integer\",\n      \"description\": \"The numeric ID of the association type\",\n      \"example\": 500123\n    }\n  },\n  \"required\": [\n    \"associationCategory\",\n    \"associationTypeId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-association-type-schema.json
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

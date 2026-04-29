---
description: Input for specifying an association type
layout: schema
name: AssociationTypeInput
properties_list:
- description: ''
  name: associationCategory
  type: string
- description: ''
  name: associationTypeId
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-association-type-input-schema.json
slug: hubspot-crm-associations-association-type-input
source_filename: hubspot-crm-associations-association-type-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for specifying an association type\",\n  \"properties\": {\n    \"associationCategory\": {\n      \"type\": \"string\",\n      \"example\": \"HUBSPOT_DEFINED\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ]\n    },\n    \"associationTypeId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    }\n  },\n  \"required\": [\n    \"associationCategory\",\n    \"associationTypeId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationTypeInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-association-type-input-schema.json
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
title: AssociationTypeInput
---

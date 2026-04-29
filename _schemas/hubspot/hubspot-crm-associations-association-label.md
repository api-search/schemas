---
description: A label that can be applied to associations
layout: schema
name: AssociationLabel
properties_list:
- description: Numeric identifier for the label type
  name: typeId
  type: integer
- description: Display text for the label
  name: label
  type: string
- description: Category of the label
  name: category
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-association-label-schema.json
slug: hubspot-crm-associations-association-label
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A label that can be applied to associations\",\n  \"properties\": {\n    \"typeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the label type\",\n      \"example\": 500123\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display text for the label\",\n      \"example\": \"Example Record\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the label\",\n      \"example\": \"HUBSPOT_DEFINED\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ]\n    }\n  },\n  \"required\": [\n    \"typeId\",\n    \"label\",\n    \"category\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationLabel\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-association-label-schema.json
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
title: AssociationLabel
---

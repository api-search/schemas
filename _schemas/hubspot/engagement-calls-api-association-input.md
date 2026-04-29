---
description: Association to create with another object
layout: schema
name: AssociationInput
properties_list:
- description: ''
  name: to
  type: object
- description: The association types
  name: types
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-association-input-schema.json
slug: engagement-calls-api-association-input
source_filename: engagement-calls-api-association-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-association-input-schema.json\",\n  \"title\": \"AssociationInput\",\n  \"description\": \"Association to create with another object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"to\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"id\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the object to associate with\",\n          \"example\": \"101\"\n        }\n      },\n      \"example\": {\n        \"id\": \"101\"\n      }\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"The association types\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Type of association\",\n        \"required\": [\n          \"associationCategory\"\
  ,\n          \"associationTypeId\"\n        ],\n        \"properties\": {\n          \"associationCategory\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HUBSPOT_DEFINED\",\n              \"USER_DEFINED\",\n              \"INTEGRATOR_DEFINED\"\n            ],\n            \"description\": \"The category of association\",\n            \"example\": \"HUBSPOT_DEFINED\"\n          },\n          \"associationTypeId\": {\n            \"type\": \"integer\",\n            \"description\": \"The association type ID\",\n            \"example\": 194\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"associationCategory\": \"HUBSPOT_DEFINED\",\n          \"associationTypeId\": 194\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"to\",\n    \"types\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-association-input-schema.json
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
title: AssociationInput
---

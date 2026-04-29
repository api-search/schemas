---
description: Input for creating an association
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
schema_file: json-schema/commerce-payments-api-association-input-schema.json
slug: commerce-payments-api-association-input
source_filename: commerce-payments-api-association-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-association-input-schema.json\",\n  \"title\": \"AssociationInput\",\n  \"description\": \"Input for creating an association\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"to\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"id\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the object to associate with\"\n        }\n      },\n      \"example\": {\n        \"id\": \"500123\"\n      }\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"The association types\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An association type definition\",\n        \"required\": [\n          \"associationCategory\",\n          \"associationTypeId\"\
  \n        ],\n        \"properties\": {\n          \"associationCategory\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HUBSPOT_DEFINED\",\n              \"USER_DEFINED\",\n              \"INTEGRATOR_DEFINED\"\n            ],\n            \"description\": \"The category of the association\",\n            \"example\": \"HUBSPOT_DEFINED\"\n          },\n          \"associationTypeId\": {\n            \"type\": \"integer\",\n            \"description\": \"The numeric ID of the association type\",\n            \"example\": 500123\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"associationCategory\": \"HUBSPOT_DEFINED\",\n          \"associationTypeId\": 500123\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"to\",\n    \"types\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-association-input-schema.json
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

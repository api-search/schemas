---
description: Represents an association between two CRM objects
layout: schema
name: Association
properties_list:
- description: ID of the target object
  name: toObjectId
  type: string
- description: Types of associations between the objects
  name: associationTypes
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-association-schema.json
slug: hubspot-crm-associations-association
source_filename: hubspot-crm-associations-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents an association between two CRM objects\",\n  \"properties\": {\n    \"toObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the target object\",\n      \"example\": \"500123\"\n    },\n    \"associationTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Types of associations between the objects\",\n      \"example\": [\n        {\n          \"associationCategory\": \"HUBSPOT_DEFINED\",\n          \"associationTypeId\": 500123,\n          \"label\": \"Example Record\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Defines the type of association\",\n        \"properties\": {\n          \"associationCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Category of the association type\",\n            \"example\": \"HUBSPOT_DEFINED\",\n            \"enum\": [\n              \"HUBSPOT_DEFINED\",\n       \
  \       \"USER_DEFINED\",\n              \"INTEGRATOR_DEFINED\"\n            ]\n          },\n          \"associationTypeId\": {\n            \"type\": \"integer\",\n            \"description\": \"Numeric identifier for the association type\",\n            \"example\": 500123\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable label for the association\",\n            \"example\": \"Example Record\"\n          }\n        },\n        \"required\": [\n          \"associationCategory\",\n          \"associationTypeId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"toObjectId\",\n    \"associationTypes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Association\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-association-schema.json
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
title: Association
---

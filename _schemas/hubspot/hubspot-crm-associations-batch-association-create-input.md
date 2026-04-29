---
description: Input for batch creating associations
layout: schema
name: BatchAssociationCreateInput
properties_list:
- description: Associations to create
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-batch-association-create-input-schema.json
slug: hubspot-crm-associations-batch-association-create-input
source_filename: hubspot-crm-associations-batch-association-create-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for batch creating associations\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Associations to create\",\n      \"example\": [\n        {\n          \"from\": {},\n          \"to\": {},\n          \"types\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Single item in a batch association create request\",\n        \"properties\": {\n          \"from\": {\n            \"type\": \"object\",\n            \"description\": \"Reference to a CRM object by ID\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"ID of the object\",\n                \"example\": \"500123\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          },\n          \"to\": {\n           \
  \ \"type\": \"object\",\n            \"description\": \"Reference to a CRM object by ID\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"ID of the object\",\n                \"example\": \"500123\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"example\": [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n                \"associationTypeId\": 500123\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"Input for specifying an association type\",\n              \"properties\": {\n                \"associationCategory\": {\n                  \"type\": \"string\",\n                  \"example\": \"HUBSPOT_DEFINED\",\n                  \"enum\": [\n             \
  \       \"HUBSPOT_DEFINED\",\n                    \"USER_DEFINED\",\n                    \"INTEGRATOR_DEFINED\"\n                  ]\n                },\n                \"associationTypeId\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                }\n              },\n              \"required\": [\n                \"associationCategory\",\n                \"associationTypeId\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"from\",\n          \"to\",\n          \"types\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchAssociationCreateInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-batch-association-create-input-schema.json
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
title: BatchAssociationCreateInput
---

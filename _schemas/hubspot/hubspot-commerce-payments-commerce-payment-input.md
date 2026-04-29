---
description: Input for creating a new commerce payment
layout: schema
name: CommercePaymentInput
properties_list:
- description: The properties to set on the commerce payment
  name: properties
  type: object
- description: Associations to create with other objects
  name: associations
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-commerce-payment-input-schema.json
slug: hubspot-commerce-payments-commerce-payment-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input for creating a new commerce payment\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties to set on the commerce payment\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"Associations to create with other objects\",\n      \"example\": [\n        {\n          \"to\": {\n            \"id\": {}\n          },\n          \"types\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for creating an association\",\n        \"properties\": {\n          \"to\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"id\": \"500123\"\n            },\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n               \
  \ \"description\": \"The ID of the object to associate with\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"description\": \"The association types\",\n            \"example\": [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n                \"associationTypeId\": 500123\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"An association type definition\",\n              \"properties\": {\n                \"associationCategory\": {\n                  \"type\": \"string\",\n                  \"description\": \"The category of the association\",\n                  \"example\": \"HUBSPOT_DEFINED\",\n                  \"enum\": [\n                    \"HUBSPOT_DEFINED\",\n                    \"USER_DEFINED\",\n                    \"INTEGRATOR_DEFINED\"\
  \n                  ]\n                },\n                \"associationTypeId\": {\n                  \"type\": \"integer\",\n                  \"description\": \"The numeric ID of the association type\",\n                  \"example\": 500123\n                }\n              },\n              \"required\": [\n                \"associationCategory\",\n                \"associationTypeId\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"to\",\n          \"types\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommercePaymentInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-commerce-payment-input-schema.json
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
title: CommercePaymentInput
---

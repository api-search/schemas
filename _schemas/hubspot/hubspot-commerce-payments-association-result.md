---
description: Association results for an object
layout: schema
name: AssociationResult
properties_list:
- description: ''
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-association-result-schema.json
slug: hubspot-commerce-payments-association-result
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Association results for an object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"type\": \"standard\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"after\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the\
  \ next page\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\"\n            }\n          }\n        },\n        \"prev\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"before\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"properties\": {\n            \"before\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the previous page\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the previous page\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-association-result-schema.json
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
title: AssociationResult
---

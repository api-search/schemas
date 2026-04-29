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
schema_file: json-schema/commerce-payments-api-association-result-schema.json
slug: commerce-payments-api-association-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-association-result-schema.json\",\n  \"title\": \"AssociationResult\",\n  \"description\": \"Association results for an object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"type\": \"standard\"\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n \
  \           \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          }\n        },\n        \"prev\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"before\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the previous page\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the previous page\"\n            }\n          },\n          \"example\": {\n            \"before\": \"example-value\",\n            \"link\": \"https://app.hubspot.com/contacts/12345\"\n          }\n        }\n      }\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-association-result-schema.json
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

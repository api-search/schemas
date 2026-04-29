---
description: A list of associations.
layout: schema
name: CollectionResponseAssociation
properties_list:
- description: ''
  name: results
  type: array
- description: Pagination information.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-deals-api-collection-response-association-schema.json
slug: crm-deals-api-collection-response-association
source_filename: crm-deals-api-collection-response-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-deals-api-collection-response-association-schema.json\",\n  \"title\": \"CollectionResponseAssociation\",\n  \"description\": \"A list of associations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An association between two CRM objects.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"type\": \"standard\"\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n     \
  \ \"description\": \"Pagination information.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-deals-api-collection-response-association-schema.json
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
title: CollectionResponseAssociation
---

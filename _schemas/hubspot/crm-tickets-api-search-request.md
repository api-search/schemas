---
description: A search request for CRM objects.
layout: schema
name: SearchRequest
properties_list:
- description: ''
  name: filterGroups
  type: array
- description: ''
  name: sorts
  type: array
- description: ''
  name: query
  type: string
- description: ''
  name: properties
  type: array
- description: ''
  name: limit
  type: integer
- description: ''
  name: after
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-tickets-api-search-request-schema.json
slug: crm-tickets-api-search-request
source_filename: crm-tickets-api-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-tickets-api-search-request-schema.json\",\n  \"title\": \"SearchRequest\",\n  \"description\": \"A search request for CRM objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of filters combined with AND logic.\",\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Filter\"\n            },\n            \"example\": [\n              {\n                \"propertyName\": \"Example Record\",\n                \"operator\": \"EQ\",\n                \"value\": \"example-value\"\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n\
  \        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ]\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"direction\": \"ASCENDING\"\n        }\n      ]\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"maximum\": 200,\n      \"example\"\
  : 100\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-tickets-api-search-request-schema.json
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
title: SearchRequest
---

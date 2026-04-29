---
description: Request body for searching commerce payments
layout: schema
name: SearchRequest
properties_list:
- description: Search query string
  name: query
  type: string
- description: Maximum number of results
  name: limit
  type: integer
- description: Pagination cursor
  name: after
  type: string
- description: Sort order for results
  name: sorts
  type: array
- description: Properties to return
  name: properties
  type: array
- description: Filter groups for the search
  name: filterGroups
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-search-request-schema.json
slug: commerce-payments-api-search-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-search-request-schema.json\",\n  \"title\": \"SearchRequest\",\n  \"description\": \"Request body for searching commerce payments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Search query string\",\n      \"example\": \"example-value\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results\",\n      \"default\": 10,\n      \"example\": 10\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination cursor\",\n      \"example\": \"example-value\"\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A sort\
  \ option for ordering results\",\n        \"required\": [\n          \"propertyName\",\n          \"direction\"\n        ],\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"description\": \"The property to sort by\",\n            \"example\": \"Example Record\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ],\n            \"description\": \"The sort direction\",\n            \"example\": \"ASCENDING\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"direction\": \"ASCENDING\"\n        }\n      ]\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to return\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n  \
  \  },\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Filter groups for the search\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of filters combined with AND logic\",\n        \"required\": [\n          \"filters\"\n        ],\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Filter\"\n            },\n            \"example\": [\n              {\n                \"propertyName\": \"Example Record\",\n                \"operator\": \"EQ\",\n                \"value\": \"example-value\",\n                \"values\": [\n                  {}\n                ],\n                \"highValue\": \"example-value\"\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-search-request-schema.json
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

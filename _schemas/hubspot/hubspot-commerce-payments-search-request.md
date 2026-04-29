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
schema_file: json-schema/hubspot-commerce-payments-search-request-schema.json
slug: hubspot-commerce-payments-search-request
source_filename: hubspot-commerce-payments-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for searching commerce payments\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Search query string\",\n      \"example\": \"example-value\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results\",\n      \"example\": 10\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination cursor\",\n      \"example\": \"example-value\"\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results\",\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"direction\": \"ASCENDING\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A sort option for ordering results\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n \
  \           \"description\": \"The property to sort by\",\n            \"example\": \"Example Record\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"description\": \"The sort direction\",\n            \"example\": \"ASCENDING\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ]\n          }\n        },\n        \"required\": [\n          \"propertyName\",\n          \"direction\"\n        ]\n      }\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to return\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Filter groups for the search\",\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"description\": \"A group of filters combined with AND logic\",\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"example\": [\n              {\n                \"propertyName\": \"Example Record\",\n                \"operator\": \"EQ\",\n                \"value\": \"example-value\",\n                \"values\": [\n                  {}\n                ],\n                \"highValue\": \"example-value\"\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"A single filter criterion\",\n              \"properties\": {\n                \"propertyName\": {\n                  \"type\": \"string\",\n                  \"description\": \"The property to filter on\",\n                  \"example\": \"Example Record\"\n                },\n                \"operator\": {\n                  \"type\": \"string\",\n                  \"description\": \"The comparison\
  \ operator\",\n                  \"example\": \"EQ\",\n                  \"enum\": [\n                    \"EQ\",\n                    \"NEQ\",\n                    \"LT\",\n                    \"LTE\",\n                    \"GT\",\n                    \"GTE\",\n                    \"BETWEEN\",\n                    \"IN\",\n                    \"NOT_IN\",\n                    \"HAS_PROPERTY\",\n                    \"NOT_HAS_PROPERTY\",\n                    \"CONTAINS_TOKEN\",\n                    \"NOT_CONTAINS_TOKEN\"\n                  ]\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The value to compare against\",\n                  \"example\": \"example-value\"\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"description\": \"Values for IN/NOT_IN operators\",\n                  \"example\": [\n                    \"example-value\"\n     \
  \             ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"highValue\": {\n                  \"type\": \"string\",\n                  \"description\": \"Upper bound for BETWEEN operator\",\n                  \"example\": \"example-value\"\n                }\n              },\n              \"required\": [\n                \"propertyName\",\n                \"operator\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"filters\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-search-request-schema.json
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

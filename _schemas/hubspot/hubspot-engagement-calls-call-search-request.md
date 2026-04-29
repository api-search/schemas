---
description: Request body for searching calls
layout: schema
name: CallSearchRequest
properties_list:
- description: Filter groups for the search (OR logic between groups)
  name: filterGroups
  type: array
- description: Sort order for results
  name: sorts
  type: array
- description: Full-text search query
  name: query
  type: string
- description: Properties to return
  name: properties
  type: array
- description: Maximum results to return
  name: limit
  type: integer
- description: Pagination cursor
  name: after
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-calls-call-search-request-schema.json
slug: hubspot-engagement-calls-call-search-request
source_filename: hubspot-engagement-calls-call-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for searching calls\",\n  \"properties\": {\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Filter groups for the search (OR logic between groups)\",\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of filters (AND logic within group)\",\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"The filters in this group\",\n            \"example\": [\n              {\n                \"propertyName\": \"hs_call_direction\",\n                \"operator\": \"EQ\",\n                \"value\": \"OUTBOUND\",\n                \"values\": [\n                  {}\n                ],\n                \"highValue\": \"example-value\"\n              }\n            ],\n            \"items\"\
  : {\n              \"type\": \"object\",\n              \"description\": \"A single search filter\",\n              \"properties\": {\n                \"propertyName\": {\n                  \"type\": \"string\",\n                  \"description\": \"The property to filter on\",\n                  \"example\": \"hs_call_direction\"\n                },\n                \"operator\": {\n                  \"type\": \"string\",\n                  \"description\": \"The filter operator\",\n                  \"example\": \"EQ\",\n                  \"enum\": [\n                    \"EQ\",\n                    \"NEQ\",\n                    \"LT\",\n                    \"LTE\",\n                    \"GT\",\n                    \"GTE\",\n                    \"BETWEEN\",\n                    \"IN\",\n                    \"NOT_IN\",\n                    \"HAS_PROPERTY\",\n                    \"NOT_HAS_PROPERTY\",\n                    \"CONTAINS_TOKEN\",\n                    \"NOT_CONTAINS_TOKEN\"\n\
  \                  ]\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The value to filter by\",\n                  \"example\": \"OUTBOUND\"\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"description\": \"Values for IN/NOT_IN operators\",\n                  \"example\": [\n                    \"example-value\"\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"highValue\": {\n                  \"type\": \"string\",\n                  \"description\": \"High value for BETWEEN operator\",\n                  \"example\": \"example-value\"\n                }\n              },\n              \"required\": [\n                \"propertyName\",\n                \"operator\"\n              ]\n            }\n          }\n        }\n      }\n    },\n\
  \    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results\",\n      \"example\": [\n        {\n          \"propertyName\": \"hs_timestamp\",\n          \"direction\": \"DESCENDING\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Sort option for search results\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"description\": \"The property to sort by\",\n            \"example\": \"hs_timestamp\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"description\": \"Sort direction\",\n            \"example\": \"DESCENDING\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ]\n          }\n        },\n        \"required\": [\n          \"propertyName\"\n        ]\n      }\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Full-text\
  \ search query\",\n      \"example\": \"discovery\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to return\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\",\n      \"example\": 10\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination cursor\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-call-search-request-schema.json
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
title: CallSearchRequest
---

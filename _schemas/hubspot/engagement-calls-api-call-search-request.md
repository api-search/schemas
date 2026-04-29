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
schema_file: json-schema/engagement-calls-api-call-search-request-schema.json
slug: engagement-calls-api-call-search-request
source_filename: engagement-calls-api-call-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-call-search-request-schema.json\",\n  \"title\": \"CallSearchRequest\",\n  \"description\": \"Request body for searching calls\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Filter groups for the search (OR logic between groups)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of filters (AND logic within group)\",\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"The filters in this group\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Filter\"\n            },\n            \"example\": [\n              {\n                \"propertyName\": \"hs_call_direction\",\n         \
  \       \"operator\": \"EQ\",\n                \"value\": \"OUTBOUND\",\n                \"values\": [\n                  {}\n                ],\n                \"highValue\": \"example-value\"\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ]\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Sort option for search results\",\n        \"required\": [\n          \"propertyName\"\n        ],\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"description\": \"The property to sort by\",\n            \"example\": \"hs_timestamp\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\
  \n            ],\n            \"description\": \"Sort direction\",\n            \"default\": \"DESCENDING\",\n            \"example\": \"DESCENDING\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"hs_timestamp\",\n          \"direction\": \"DESCENDING\"\n        }\n      ]\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Full-text search query\",\n      \"example\": \"discovery\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Properties to return\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\",\n      \"default\": 10,\n      \"maximum\": 100,\n      \"example\": 10\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination cursor\",\n      \"example\": \"\
  example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-call-search-request-schema.json
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

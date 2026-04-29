---
description: A search request for CRM objects. Filter groups are combined with OR logic; filters within a group are combined with AND logic.
layout: schema
name: SearchRequest
properties_list:
- description: An array of filter groups. Records matching any filter group will be included in results (OR logic between groups). Filters within a group are all required (AND logic within groups).
  name: filterGroups
  type: array
- description: An array of sort criteria to order the results.
  name: sorts
  type: array
- description: A full-text search query string. When provided, returns records where any searchable property contains the query term.
  name: query
  type: string
- description: An array of property names to include in the response for each record. If not specified, a default set of properties is returned.
  name: properties
  type: array
- description: The maximum number of results to return. Maximum value is 200.
  name: limit
  type: integer
- description: The cursor token for pagination. Use the value from the previous response's paging.next.after to get the next page of results.
  name: after
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-search-api-search-request-schema.json
slug: crm-search-api-search-request
source_filename: crm-search-api-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-search-request-schema.json\",\n  \"title\": \"SearchRequest\",\n  \"description\": \"A search request for CRM objects. Filter groups are combined with OR logic; filters within a group are combined with AND logic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"An array of filter groups. Records matching any filter group will be included in results (OR logic between groups). Filters within a group are all required (AND logic within groups).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of filter conditions combined with AND logic. Use multiple filter groups to create OR conditions between groups.\",\n        \"properties\": {\n          \"filters\": {\n            \"type\":\
  \ \"array\",\n            \"description\": \"An array of filters, all of which must match (AND logic).\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Filter\"\n            },\n            \"example\": [\n              {\n                \"propertyName\": \"Example Record\",\n                \"operator\": \"EQ\",\n                \"value\": \"example-value\",\n                \"highValue\": \"example-value\",\n                \"values\": [\n                  {}\n                ]\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ]\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"An array of sort criteria to order the results.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A sort criterion for ordering search results.\",\n        \"required\": [\n          \"propertyName\"\n\
  \        ],\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the CRM property to sort by.\",\n            \"example\": \"Example Record\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"description\": \"The sort direction.\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ],\n            \"default\": \"ASCENDING\",\n            \"example\": \"ASCENDING\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"direction\": \"ASCENDING\"\n        }\n      ]\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"A full-text search query string. When provided, returns records where any searchable property contains the query term.\",\n      \"example\": \"example-value\"\n    },\n    \"properties\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"An array of property names to include in the response for each record. If not specified, a default set of properties is returned.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to return. Maximum value is 200.\",\n      \"default\": 10,\n      \"maximum\": 200,\n      \"example\": 10\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor token for pagination. Use the value from the previous response's paging.next.after to get the next page of results.\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-search-api-search-request-schema.json
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

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
schema_file: json-schema/hubspot-crm-search-search-request-schema.json
slug: hubspot-crm-search-search-request
source_filename: hubspot-crm-search-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A search request for CRM objects. Filter groups are combined with OR logic; filters within a group are combined with AND logic.\",\n  \"properties\": {\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"An array of filter groups. Records matching any filter group will be included in results (OR logic between groups). Filters within a group are all required (AND logic within groups).\",\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group of filter conditions combined with AND logic. Use multiple filter groups to create OR conditions between groups.\",\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"An array of filters, all of which must match (AND logic).\",\n            \"example\": [\n\
  \              {\n                \"propertyName\": \"Example Record\",\n                \"operator\": \"EQ\",\n                \"value\": \"example-value\",\n                \"highValue\": \"example-value\",\n                \"values\": [\n                  {}\n                ]\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"A single filter condition for a CRM object property.\",\n              \"properties\": {\n                \"propertyName\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the CRM property to filter on.\",\n                  \"example\": \"Example Record\"\n                },\n                \"operator\": {\n                  \"type\": \"string\",\n                  \"description\": \"The comparison operator for the filter.\",\n                  \"example\": \"EQ\",\n                  \"enum\": [\n                    \"EQ\",\n          \
  \          \"NEQ\",\n                    \"LT\",\n                    \"LTE\",\n                    \"GT\",\n                    \"GTE\",\n                    \"BETWEEN\",\n                    \"IN\",\n                    \"NOT_IN\",\n                    \"HAS_PROPERTY\",\n                    \"NOT_HAS_PROPERTY\",\n                    \"CONTAINS_TOKEN\",\n                    \"NOT_CONTAINS_TOKEN\"\n                  ]\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The value to compare against. Not required for HAS_PROPERTY and NOT_HAS_PROPERTY operators.\",\n                  \"example\": \"example-value\"\n                },\n                \"highValue\": {\n                  \"type\": \"string\",\n                  \"description\": \"The upper bound value for BETWEEN operator comparisons.\",\n                  \"example\": \"example-value\"\n                },\n                \"values\": {\n         \
  \         \"type\": \"array\",\n                  \"description\": \"An array of values for IN and NOT_IN operator comparisons.\",\n                  \"example\": [\n                    \"example-value\"\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"propertyName\",\n                \"operator\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"An array of sort criteria to order the results.\",\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"direction\": \"ASCENDING\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A sort criterion for ordering search results.\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\"\
  : \"string\",\n            \"description\": \"The name of the CRM property to sort by.\",\n            \"example\": \"Example Record\"\n          },\n          \"direction\": {\n            \"type\": \"string\",\n            \"description\": \"The sort direction.\",\n            \"example\": \"ASCENDING\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ]\n          }\n        },\n        \"required\": [\n          \"propertyName\"\n        ]\n      }\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"A full-text search query string. When provided, returns records where any searchable property contains the query term.\",\n      \"example\": \"example-value\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"An array of property names to include in the response for each record. If not specified, a default set of properties is returned.\",\n      \"example\": [\n        \"example-value\"\
  \n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to return. Maximum value is 200.\",\n      \"example\": 10\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor token for pagination. Use the value from the previous response's paging.next.after to get the next page of results.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-search-search-request-schema.json
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

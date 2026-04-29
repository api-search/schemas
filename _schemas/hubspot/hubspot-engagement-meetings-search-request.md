---
description: ''
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
schema_file: json-schema/hubspot-engagement-meetings-search-request-schema.json
slug: hubspot-engagement-meetings-search-request
source_filename: hubspot-engagement-meetings-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterGroups\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"filters\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"filters\": {\n            \"type\": \"array\",\n            \"example\": [\n              {\n                \"propertyName\": \"Example Record\",\n                \"operator\": \"EQ\",\n                \"value\": \"example-value\"\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"propertyName\": {\n                  \"type\": \"string\",\n                  \"example\": \"Example Record\"\n                },\n                \"operator\": {\n                  \"type\": \"string\",\n                  \"example\": \"EQ\",\n                  \"enum\": [\n                    \"EQ\",\n \
  \                   \"NEQ\",\n                    \"LT\",\n                    \"LTE\",\n                    \"GT\",\n                    \"GTE\",\n                    \"BETWEEN\",\n                    \"IN\",\n                    \"NOT_IN\",\n                    \"HAS_PROPERTY\",\n                    \"NOT_HAS_PROPERTY\",\n                    \"CONTAINS_TOKEN\",\n                    \"NOT_CONTAINS_TOKEN\"\n                  ]\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"example\": \"example-value\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"propertyName\": \"Example Record\",\n          \"direction\": \"ASCENDING\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"propertyName\": {\n            \"type\": \"string\"\n  \
  \        },\n          \"direction\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ASCENDING\",\n              \"DESCENDING\"\n            ]\n          }\n        }\n      }\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"example-value\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"after\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-meetings-search-request-schema.json
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

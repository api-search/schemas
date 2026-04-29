---
description: List of basic metrics
layout: schema
name: Metrics
properties_list:
- description: Data used for charting etc
  name: datasets
  type: array
- description: Percentage of all APIs where auto fixes have been applied
  name: fixedPct
  type: integer
- description: Total number of fixes applied across all APIs
  name: fixes
  type: integer
- description: Number of newly invalid APIs
  name: invalid
  type: integer
- description: Open GitHub issues on our main repo
  name: issues
  type: integer
- description: Number of unique APIs
  name: numAPIs
  type: integer
- description: Number of methods of API retrieval
  name: numDrivers
  type: integer
- description: Total number of endpoints inside all definitions
  name: numEndpoints
  type: integer
- description: Number of API providers in directory
  name: numProviders
  type: integer
- description: Number of API definitions including different versions of the same API
  name: numSpecs
  type: integer
- description: GitHub stars for our main repo
  name: stars
  type: integer
- description: Summary totals for the last 7 days
  name: thisWeek
  type: object
- description: Number of unofficial APIs
  name: unofficial
  type: integer
- description: Number of unreachable (4XX,5XX status) APIs
  name: unreachable
  type: integer
provider_name: APIs.guru
provider_slug: apis-guru
schema_file: json-schema/apis-guru-metrics-schema.json
slug: apis-guru-metrics
source_filename: apis-guru-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-metrics-schema.json\",\n  \"title\": \"Metrics\",\n  \"description\": \"List of basic metrics\",\n  \"additionalProperties\": false,\n  \"example\": {\n    \"datasets\": [],\n    \"fixedPct\": 22,\n    \"fixes\": 81119,\n    \"invalid\": 598,\n    \"issues\": 28,\n    \"numAPIs\": 2501,\n    \"numDrivers\": 10,\n    \"numEndpoints\": 106448,\n    \"numProviders\": 659,\n    \"numSpecs\": 3329,\n    \"stars\": 2429,\n    \"thisWeek\": {\n      \"added\": 45,\n      \"updated\": 171\n    },\n    \"unofficial\": 25,\n    \"unreachable\": 123\n  },\n  \"properties\": {\n    \"datasets\": {\n      \"description\": \"Data used for charting etc\",\n      \"items\": {},\n      \"type\": \"array\"\n    },\n    \"fixedPct\": {\n      \"description\": \"Percentage of all APIs where auto fixes have been applied\"\
  ,\n      \"type\": \"integer\"\n    },\n    \"fixes\": {\n      \"description\": \"Total number of fixes applied across all APIs\",\n      \"type\": \"integer\"\n    },\n    \"invalid\": {\n      \"description\": \"Number of newly invalid APIs\",\n      \"type\": \"integer\"\n    },\n    \"issues\": {\n      \"description\": \"Open GitHub issues on our main repo\",\n      \"type\": \"integer\"\n    },\n    \"numAPIs\": {\n      \"description\": \"Number of unique APIs\",\n      \"minimum\": 1,\n      \"type\": \"integer\"\n    },\n    \"numDrivers\": {\n      \"description\": \"Number of methods of API retrieval\",\n      \"type\": \"integer\"\n    },\n    \"numEndpoints\": {\n      \"description\": \"Total number of endpoints inside all definitions\",\n      \"minimum\": 1,\n      \"type\": \"integer\"\n    },\n    \"numProviders\": {\n      \"description\": \"Number of API providers in directory\",\n      \"type\": \"integer\"\n    },\n    \"numSpecs\": {\n      \"description\": \"Number\
  \ of API definitions including different versions of the same API\",\n      \"minimum\": 1,\n      \"type\": \"integer\"\n    },\n    \"stars\": {\n      \"description\": \"GitHub stars for our main repo\",\n      \"type\": \"integer\"\n    },\n    \"thisWeek\": {\n      \"description\": \"Summary totals for the last 7 days\",\n      \"properties\": {\n        \"added\": {\n          \"description\": \"APIs added in the last week\",\n          \"type\": \"integer\"\n        },\n        \"updated\": {\n          \"description\": \"APIs updated in the last week\",\n          \"type\": \"integer\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"unofficial\": {\n      \"description\": \"Number of unofficial APIs\",\n      \"type\": \"integer\"\n    },\n    \"unreachable\": {\n      \"description\": \"Number of unreachable (4XX,5XX status) APIs\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"numSpecs\",\n    \"numAPIs\",\n    \"numEndpoints\"\n  ],\n \
  \ \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-metrics-schema.json
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
title: Metrics
---

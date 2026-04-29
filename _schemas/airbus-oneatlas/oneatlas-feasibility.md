---
description: ''
layout: schema
name: Feasibility
properties_list:
- description: ''
  name: progCapacities
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-feasibility-schema.json
slug: oneatlas-feasibility
source_filename: oneatlas-feasibility-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-feasibility-schema.json\",\n  \"title\": \"Feasibility\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"progCapacities\": {\n      \"items\": {\n        \"properties\": {\n          \"mission\": {\n            \"enum\": [\n              \"PLEIADESNEO\"\n            ],\n            \"type\": \"string\"\n          },\n          \"progTypes\": {\n            \"items\": {\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"mission\": {\n                  \"enum\": [\n                    \"PLEIADESNEO\"\n                  ],\n                  \"type\": \"string\"\n                },\n                \"feasibility\": {\n                  \"properties\": {\n                    \"automation\": {\n        \
  \              \"description\": \"To be used when creating the order and/or requesting the quotation\",\n                      \"enum\": [\n                        \"AUTOMATIC\",\n                        \"MANUAL\"\n                      ],\n                      \"type\": \"string\"\n                    },\n                    \"classification\": {\n                      \"description\": \"To be used when creating the order and/or requesting the quotation\",\n                      \"enum\": [\n                        \"CHALLENGING\",\n                        \"EASY\"\n                      ],\n                      \"type\": \"string\"\n                    }\n                  },\n                  \"type\": \"object\"\n                },\n                \"available\": {\n                  \"type\": \"boolean\"\n                },\n                \"expirationDate\": {\n                  \"format\": \"datetime\",\n                  \"type\": \"string\"\n                }\n          \
  \    },\n              \"type\": \"object\"\n            },\n            \"type\": \"array\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-feasibility-schema.json
tags:
- Imagery
- Satellites
title: Feasibility
---

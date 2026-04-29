---
description: ''
layout: schema
name: ListReadSetsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: readSets
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-read-sets-response-schema.json
slug: healthomics-list-read-sets-response
source_filename: healthomics-list-read-sets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-sets-response-schema.json\",\n  \"title\": \"ListReadSetsResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"readSets\"\n  ],\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"readSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetList\"\n        },\n        {\n          \"description\": \"A list of read sets.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-sets-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReadSetsResponse
---

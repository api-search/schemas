---
description: ''
layout: schema
name: ListSequenceStoresResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: sequenceStores
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-sequence-stores-response-schema.json
slug: healthomics-list-sequence-stores-response
source_filename: healthomics-list-sequence-stores-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-sequence-stores-response-schema.json\",\n  \"title\": \"ListSequenceStoresResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sequenceStores\"\n  ],\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"sequenceStores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreDetailList\"\n        },\n        {\n          \"description\": \"A list of sequence stores.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-sequence-stores-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListSequenceStoresResponse
---

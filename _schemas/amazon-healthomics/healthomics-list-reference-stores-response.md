---
description: ''
layout: schema
name: ListReferenceStoresResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: referenceStores
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-reference-stores-response-schema.json
slug: healthomics-list-reference-stores-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-reference-stores-response-schema.json\",\n  \"title\": \"ListReferenceStoresResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"referenceStores\"\n  ],\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"referenceStores\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreDetailList\"\n        },\n        {\n          \"description\": \"A list of reference stores.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-reference-stores-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReferenceStoresResponse
---

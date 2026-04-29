---
description: ''
layout: schema
name: ListReferencesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: references
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-references-response-schema.json
slug: healthomics-list-references-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-references-response-schema.json\",\n  \"title\": \"ListReferencesResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"references\"\n  ],\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"references\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceList\"\n        },\n        {\n          \"description\": \"A list of references.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-references-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReferencesResponse
---

---
description: A filter for annotation stores.
layout: schema
name: ListAnnotationStoresFilter
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-annotation-stores-filter-schema.json
slug: healthomics-list-annotation-stores-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-stores-filter-schema.json\",\n  \"title\": \"ListAnnotationStoresFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreStatus\"\n        },\n        {\n          \"description\": \"A status to filter on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A filter for annotation stores.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-annotation-stores-filter-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListAnnotationStoresFilter
---

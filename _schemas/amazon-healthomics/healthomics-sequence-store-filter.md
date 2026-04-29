---
description: A filter for a sequence store.
layout: schema
name: SequenceStoreFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: createdAfter
  type: object
- description: ''
  name: createdBefore
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-sequence-store-filter-schema.json
slug: healthomics-sequence-store-filter
source_filename: healthomics-sequence-store-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sequence-store-filter-schema.json\",\n  \"title\": \"SequenceStoreFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreName\"\n        },\n        {\n          \"description\": \"A name to filter on.\"\n        }\n      ]\n    },\n    \"createdAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's start date.\"\n        }\n      ]\n    },\n    \"createdBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's end date.\"\n        }\n\
  \      ]\n    }\n  },\n  \"description\": \"A filter for a sequence store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sequence-store-filter-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: SequenceStoreFilter
---

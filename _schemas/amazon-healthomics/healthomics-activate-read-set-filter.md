---
description: A read set activation job filter.
layout: schema
name: ActivateReadSetFilter
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: createdAfter
  type: object
- description: ''
  name: createdBefore
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-activate-read-set-filter-schema.json
slug: healthomics-activate-read-set-filter
source_filename: healthomics-activate-read-set-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-activate-read-set-filter-schema.json\",\n  \"title\": \"ActivateReadSetFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetActivationJobStatus\"\n        },\n        {\n          \"description\": \"The filter's status.\"\n        }\n      ]\n    },\n    \"createdAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's start date.\"\n        }\n      ]\n    },\n    \"createdBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's end date.\"\
  \n        }\n      ]\n    }\n  },\n  \"description\": \"A read set activation job filter.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-activate-read-set-filter-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ActivateReadSetFilter
---

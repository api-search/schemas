---
description: A filter for import read set jobs.
layout: schema
name: ImportReadSetFilter
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
schema_file: json-schema/healthomics-import-read-set-filter-schema.json
slug: healthomics-import-read-set-filter
source_filename: healthomics-import-read-set-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-import-read-set-filter-schema.json\",\n  \"title\": \"ImportReadSetFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetImportJobStatus\"\n        },\n        {\n          \"description\": \"A status to filter on.\"\n        }\n      ]\n    },\n    \"createdAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's start date.\"\n        }\n      ]\n    },\n    \"createdBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's end date.\"\n\
  \        }\n      ]\n    }\n  },\n  \"description\": \"A filter for import read set jobs.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-import-read-set-filter-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ImportReadSetFilter
---

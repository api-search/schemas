---
description: An read set export job filter.
layout: schema
name: ExportReadSetFilter
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
schema_file: json-schema/healthomics-export-read-set-filter-schema.json
slug: healthomics-export-read-set-filter
source_filename: healthomics-export-read-set-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-filter-schema.json\",\n  \"title\": \"ExportReadSetFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetExportJobStatus\"\n        },\n        {\n          \"description\": \"A status to filter on.\"\n        }\n      ]\n    },\n    \"createdAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's start date.\"\n        }\n      ]\n    },\n    \"createdBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The filter's end date.\"\n\
  \        }\n      ]\n    }\n  },\n  \"description\": \"An read set export job filter.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-filter-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ExportReadSetFilter
---

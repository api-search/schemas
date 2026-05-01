---
description: Filter settings that select for read set upload parts of interest.
layout: schema
name: ReadSetUploadPartListFilter
properties_list:
- description: ''
  name: createdAfter
  type: object
- description: ''
  name: createdBefore
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-read-set-upload-part-list-filter-schema.json
slug: healthomics-read-set-upload-part-list-filter
source_filename: healthomics-read-set-upload-part-list-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-upload-part-list-filter-schema.json\",\n  \"title\": \"ReadSetUploadPartListFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \" Filters for read set uploads after a specified time. \"\n        }\n      ]\n    },\n    \"createdBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \" Filters for read set part uploads before a specified time. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" Filter settings that select for read set upload parts of interest. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-upload-part-list-filter-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReadSetUploadPartListFilter
---

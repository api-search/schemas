---
description: A single row returned by a BJS Socrata-backed dataset (NCVS or NIBRS National Estimates). Field names and types vary per dataset; common metadata fields are described below.
layout: schema
name: BJSDatasetRow
properties_list:
- description: Survey or reporting year associated with the row.
  name: year
  type: string
- description: Numeric estimate as published by BJS, returned as a string.
  name: estimate
  type: string
- description: Standard error of the estimate where applicable.
  name: standard_error
  type: string
- description: Category, demographic, or offense grouping for the estimate.
  name: category
  type: string
provider_name: Bureau of Justice Statistics Data Analysis Tools
provider_slug: data-analysis-tools-bureau-of-justice-statistics
schema_file: json-schema/bjs-dataset-row.json
slug: bjs-dataset-row
source_filename: bjs-dataset-row.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/json-schema/bjs-dataset-row.json\",\n  \"title\": \"BJSDatasetRow\",\n  \"description\": \"A single row returned by a BJS Socrata-backed dataset (NCVS or NIBRS National Estimates). Field names and types vary per dataset; common metadata fields are described below.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"year\": {\n      \"type\": \"string\",\n      \"description\": \"Survey or reporting year associated with the row.\"\n    },\n    \"estimate\": {\n      \"type\": \"string\",\n      \"description\": \"Numeric estimate as published by BJS, returned as a string.\"\n    },\n    \"standard_error\": {\n      \"type\": \"string\",\n      \"description\": \"Standard error of the estimate where applicable.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Category, demographic, or offense grouping for the estimate.\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/json-schema/bjs-dataset-row.json
tags:
- Crime Statistics
- Federal Government
- NCVS
- NIBRS
- Open Data
- SODA
- Statistics
- Victimization
title: BJSDatasetRow
---

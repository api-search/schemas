---
description: List of job postings.
layout: schema
name: JobsResponse
properties_list:
- description: Array of job postings.
  name: data
  type: array
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-jobs-response-schema.json
slug: bindbee-jobs-response
source_filename: bindbee-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"JobsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of job postings.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of job postings.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Job\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-jobs-response-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: JobsResponse
---

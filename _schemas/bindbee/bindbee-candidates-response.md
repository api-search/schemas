---
description: List of candidates.
layout: schema
name: CandidatesResponse
properties_list:
- description: Array of candidate records.
  name: data
  type: array
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-candidates-response-schema.json
slug: bindbee-candidates-response
source_filename: bindbee-candidates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CandidatesResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of candidates.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of candidate records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Candidate\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-candidates-response-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: CandidatesResponse
---

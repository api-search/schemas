---
description: Equal Employment Opportunity (EEO) compliance responses provided by the candidate. Available only for US employers with EEO questions enabled.
layout: schema
name: EeoResponses
properties_list:
- description: The candidate's self-reported gender identity.
  name: gender
  type: string
- description: The candidate's self-reported race or ethnicity.
  name: race
  type: string
- description: The candidate's veteran status.
  name: veteranStatus
  type: string
- description: The candidate's disability status.
  name: disabilityStatus
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-eeo-responses-schema.json
slug: indeed-employer-eeo-responses
source_filename: indeed-employer-eeo-responses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EeoResponses\",\n  \"type\": \"object\",\n  \"description\": \"Equal Employment Opportunity (EEO) compliance responses provided by the candidate. Available only for US employers with EEO questions enabled.\",\n  \"properties\": {\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's self-reported gender identity.\"\n    },\n    \"race\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's self-reported race or ethnicity.\"\n    },\n    \"veteranStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's veteran status.\"\n    },\n    \"disabilityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's disability status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-eeo-responses-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: EeoResponses
---

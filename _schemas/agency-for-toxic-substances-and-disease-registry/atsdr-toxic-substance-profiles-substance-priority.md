---
description: SubstancePriority schema from ATSDR API
layout: schema
name: SubstancePriority
properties_list:
- description: Priority rank on the ATSDR Substance Priority List.
  name: rank
  type: integer
- description: Name of the substance.
  name: substance_name
  type: string
- description: CAS registry number.
  name: cas_number
  type: string
- description: Composite score used for ranking.
  name: total_score
  type: number
- description: Number of NPL sites where substance was found.
  name: npl_frequency
  type: integer
- description: Toxicity component of the score.
  name: toxicity_score
  type: number
- description: Priority list year.
  name: year
  type: integer
provider_name: Agency for Toxic Substances and Disease Registry
provider_slug: agency-for-toxic-substances-and-disease-registry
schema_file: json-schema/atsdr-toxic-substance-profiles-substance-priority-schema.json
slug: atsdr-toxic-substance-profiles-substance-priority
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-substance-priority-schema.json\",\n  \"title\": \"SubstancePriority\",\n  \"description\": \"SubstancePriority schema from ATSDR API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rank\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority rank on the ATSDR Substance Priority List.\",\n      \"example\": 1\n    },\n    \"substance_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the substance.\",\n      \"example\": \"Example Name\"\n    },\n    \"cas_number\": {\n      \"type\": \"string\",\n      \"description\": \"CAS registry number.\",\n      \"example\": \"example_value\"\n    },\n    \"total_score\": {\n      \"type\": \"number\",\n      \"description\": \"Composite score used for ranking.\"\
  ,\n      \"example\": 99.99\n    },\n    \"npl_frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of NPL sites where substance was found.\",\n      \"example\": 1\n    },\n    \"toxicity_score\": {\n      \"type\": \"number\",\n      \"description\": \"Toxicity component of the score.\",\n      \"example\": 99.99\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority list year.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-substance-priority-schema.json
tags:
- Diseases
- Federal Government
- Public Health
- Toxic Substances
- Environmental Health
- Hazardous Materials
title: SubstancePriority
---

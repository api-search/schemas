---
description: ToxProfile schema from ATSDR API
layout: schema
name: ToxProfile
properties_list:
- description: Name of the hazardous substance.
  name: substance_name
  type: string
- description: Chemical Abstracts Service registry number.
  name: cas_number
  type: string
- description: Year the toxicological profile was published or updated.
  name: profile_year
  type: integer
- description: Rank on the ATSDR Substance Priority List.
  name: substance_priority_list_rank
  type: integer
- description: Summary of known health effects from exposure.
  name: health_effects
  type: string
- description: Most common route of exposure (ingestion, inhalation, dermal).
  name: primary_route_of_exposure
  type: string
- description: URL to the full toxicological profile PDF.
  name: profile_url
  type: string
provider_name: Agency for Toxic Substances and Disease Registry
provider_slug: agency-for-toxic-substances-and-disease-registry
schema_file: json-schema/atsdr-toxic-substance-profiles-tox-profile-schema.json
slug: atsdr-toxic-substance-profiles-tox-profile
source_filename: atsdr-toxic-substance-profiles-tox-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-tox-profile-schema.json\",\n  \"title\": \"ToxProfile\",\n  \"description\": \"ToxProfile schema from ATSDR API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"substance_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the hazardous substance.\",\n      \"example\": \"Example Name\"\n    },\n    \"cas_number\": {\n      \"type\": \"string\",\n      \"description\": \"Chemical Abstracts Service registry number.\",\n      \"example\": \"example_value\"\n    },\n    \"profile_year\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the toxicological profile was published or updated.\",\n      \"example\": 1\n    },\n    \"substance_priority_list_rank\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Rank on the ATSDR Substance Priority List.\",\n      \"example\": 1\n    },\n    \"health_effects\": {\n      \"type\": \"string\",\n      \"description\": \"Summary of known health effects from exposure.\",\n      \"example\": \"example_value\"\n    },\n    \"primary_route_of_exposure\": {\n      \"type\": \"string\",\n      \"description\": \"Most common route of exposure (ingestion, inhalation, dermal).\",\n      \"example\": \"example_value\"\n    },\n    \"profile_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the full toxicological profile PDF.\",\n      \"example\": \"https://example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-tox-profile-schema.json
tags:
- Diseases
- Federal Government
- Public Health
- Toxic Substances
- Environmental Health
- Hazardous Materials
title: ToxProfile
---

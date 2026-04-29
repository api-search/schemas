---
description: MinimumRiskLevel schema from ATSDR API
layout: schema
name: MinimumRiskLevel
properties_list:
- description: Name of the hazardous substance.
  name: substance_name
  type: string
- description: CAS registry number.
  name: cas_number
  type: string
- description: Exposure route.
  name: route
  type: string
- description: Duration of exposure.
  name: duration
  type: string
- description: MRL value (units depend on route).
  name: mrl_value
  type: number
- description: Unit of measurement for the MRL value.
  name: mrl_unit
  type: string
- description: Year the MRL was last updated.
  name: year_updated
  type: integer
provider_name: Agency for Toxic Substances and Disease Registry
provider_slug: agency-for-toxic-substances-and-disease-registry
schema_file: json-schema/atsdr-toxic-substance-profiles-minimum-risk-level-schema.json
slug: atsdr-toxic-substance-profiles-minimum-risk-level
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-minimum-risk-level-schema.json\",\n  \"title\": \"MinimumRiskLevel\",\n  \"description\": \"MinimumRiskLevel schema from ATSDR API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"substance_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the hazardous substance.\",\n      \"example\": \"Example Name\"\n    },\n    \"cas_number\": {\n      \"type\": \"string\",\n      \"description\": \"CAS registry number.\",\n      \"example\": \"example_value\"\n    },\n    \"route\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"inhalation\",\n        \"oral\",\n        \"dermal\"\n      ],\n      \"description\": \"Exposure route.\",\n      \"example\": \"inhalation\"\n    },\n    \"duration\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\n        \"acute\",\n        \"intermediate\",\n        \"chronic\"\n      ],\n      \"description\": \"Duration of exposure.\",\n      \"example\": \"acute\"\n    },\n    \"mrl_value\": {\n      \"type\": \"number\",\n      \"description\": \"MRL value (units depend on route).\",\n      \"example\": 99.99\n    },\n    \"mrl_unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement for the MRL value.\",\n      \"example\": \"example_value\"\n    },\n    \"year_updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Year the MRL was last updated.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-minimum-risk-level-schema.json
tags:
- Diseases
- Federal Government
- Public Health
- Toxic Substances
- Environmental Health
- Hazardous Materials
title: MinimumRiskLevel
---

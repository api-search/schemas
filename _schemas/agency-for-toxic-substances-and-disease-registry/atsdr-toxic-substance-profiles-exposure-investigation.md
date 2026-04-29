---
description: ExposureInvestigation schema from ATSDR API
layout: schema
name: ExposureInvestigation
properties_list:
- description: Name of the contaminated site.
  name: site_name
  type: string
- description: US state abbreviation.
  name: state
  type: string
- description: County name.
  name: county
  type: string
- description: Year of the investigation.
  name: year
  type: integer
- description: Type of investigation (Health Consultation, Public Health Assessment, etc.).
  name: investigation_type
  type: string
- description: Primary hazardous substance involved.
  name: primary_contaminant
  type: string
- description: Investigation status.
  name: status
  type: string
provider_name: Agency for Toxic Substances and Disease Registry
provider_slug: agency-for-toxic-substances-and-disease-registry
schema_file: json-schema/atsdr-toxic-substance-profiles-exposure-investigation-schema.json
slug: atsdr-toxic-substance-profiles-exposure-investigation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-exposure-investigation-schema.json\",\n  \"title\": \"ExposureInvestigation\",\n  \"description\": \"ExposureInvestigation schema from ATSDR API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the contaminated site.\",\n      \"example\": \"Example Name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state abbreviation.\",\n      \"example\": \"example_value\"\n    },\n    \"county\": {\n      \"type\": \"string\",\n      \"description\": \"County name.\",\n      \"example\": \"example_value\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Year of the investigation.\",\n      \"example\"\
  : 1\n    },\n    \"investigation_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of investigation (Health Consultation, Public Health Assessment, etc.).\",\n      \"example\": \"example_value\"\n    },\n    \"primary_contaminant\": {\n      \"type\": \"string\",\n      \"description\": \"Primary hazardous substance involved.\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"completed\",\n        \"ongoing\",\n        \"pending\"\n      ],\n      \"description\": \"Investigation status.\",\n      \"example\": \"completed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agency-for-toxic-substances-and-disease-registry/refs/heads/main/json-schema/atsdr-toxic-substance-profiles-exposure-investigation-schema.json
tags:
- Diseases
- Federal Government
- Public Health
- Toxic Substances
- Environmental Health
- Hazardous Materials
title: ExposureInvestigation
---

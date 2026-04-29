---
description: Schema for the JSON object returned by Climatiq estimation endpoints. An emission estimate quantifies CO2-equivalent emissions for a single activity by combining a chosen emission factor with caller-supplied activity parameters such as energy used, distance travelled, money spent, or weight moved.
layout: schema
name: Climatiq Emission Estimate
properties_list:
- description: Total CO2-equivalent emissions for the activity, expressed in co2e_unit.
  name: co2e
  type: number
- description: Unit of measure for co2e (typically 'kg').
  name: co2e_unit
  type: string
- description: Calculation methodology used for the estimate (for example, ar4, ar5, ar6).
  name: co2e_calculation_method
  type: string
- description: Source of the calculation (for example, source for factors derived directly from a referenced source).
  name: co2e_calculation_origin
  type: string
- description: Metadata describing the emission factor used to produce this estimate.
  name: emission_factor
  type: object
- description: Breakdown of the estimate into constituent greenhouse gases.
  name: constituent_gases
  type: object
- description: Echo of the activity inputs used in the calculation.
  name: activity_data
  type: object
- description: Reference to the audit-trail entry recorded for this estimate when audit-trail is enabled.
  name: audit_trail
  type: string
provider_name: Climatiq
provider_slug: climatiq
schema_file: json-schema/climatiq-emission-estimate-schema.json
slug: climatiq-emission-estimate
source_filename: climatiq-emission-estimate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.climatiq.io/schemas/emission-estimate.json\",\n  \"title\": \"Climatiq Emission Estimate\",\n  \"description\": \"Schema for the JSON object returned by Climatiq estimation endpoints. An emission estimate quantifies CO2-equivalent emissions for a single activity by combining a chosen emission factor with caller-supplied activity parameters such as energy used, distance travelled, money spent, or weight moved.\",\n  \"type\": \"object\",\n  \"required\": [\"co2e\", \"co2e_unit\"],\n  \"properties\": {\n    \"co2e\": {\n      \"type\": \"number\",\n      \"description\": \"Total CO2-equivalent emissions for the activity, expressed in co2e_unit.\"\n    },\n    \"co2e_unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure for co2e (typically 'kg').\",\n      \"examples\": [\"kg\"]\n    },\n    \"co2e_calculation_method\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Calculation methodology used for the estimate (for example, ar4, ar5, ar6).\",\n      \"enum\": [\"ar4\", \"ar5\", \"ar6\"]\n    },\n    \"co2e_calculation_origin\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the calculation (for example, source for factors derived directly from a referenced source).\"\n    },\n    \"emission_factor\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata describing the emission factor used to produce this estimate.\",\n      \"properties\": {\n        \"name\": {\"type\": \"string\"},\n        \"activity_id\": {\"type\": \"string\"},\n        \"id\": {\"type\": \"string\"},\n        \"access_type\": {\"type\": \"string\"},\n        \"source\": {\"type\": \"string\"},\n        \"source_dataset\": {\"type\": \"string\"},\n        \"year\": {\"type\": \"integer\"},\n        \"region\": {\"type\": \"string\"},\n        \"category\": {\"type\": \"string\"},\n        \"source_lca_activity\": {\"type\"\
  : \"string\"},\n        \"data_quality_flags\": {\n          \"type\": \"array\",\n          \"items\": {\"type\": \"string\"}\n        }\n      }\n    },\n    \"constituent_gases\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of the estimate into constituent greenhouse gases.\",\n      \"properties\": {\n        \"co2e_total\": {\"type\": [\"number\", \"null\"]},\n        \"co2e_other\": {\"type\": [\"number\", \"null\"]},\n        \"co2\": {\"type\": [\"number\", \"null\"]},\n        \"ch4\": {\"type\": [\"number\", \"null\"]},\n        \"n2o\": {\"type\": [\"number\", \"null\"]}\n      }\n    },\n    \"activity_data\": {\n      \"type\": \"object\",\n      \"description\": \"Echo of the activity inputs used in the calculation.\",\n      \"properties\": {\n        \"activity_value\": {\"type\": \"number\"},\n        \"activity_unit\": {\"type\": \"string\"}\n      }\n    },\n    \"audit_trail\": {\n      \"type\": \"string\",\n      \"description\": \"Reference\
  \ to the audit-trail entry recorded for this estimate when audit-trail is enabled.\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/json-schema/climatiq-emission-estimate-schema.json
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Energy
- Environment
- GHG Protocol
- Sustainability
title: Climatiq Emission Estimate
---

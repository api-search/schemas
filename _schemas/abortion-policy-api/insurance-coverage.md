---
description: Abortion insurance coverage restrictions covering Medicaid, private insurance, and ACA exchange plans for a US state.
layout: schema
name: InsuranceCoverage
properties_list:
- description: If true, state requires private health plans to cover abortion.
  name: requires_coverage
  type: boolean
- description: If true, private insurance may cover abortion without restrictions.
  name: private_coverage_no_restrictions
  type: boolean
- description: If true, private insurance coverage allowed when abortion is necessary to save pregnant person's life.
  name: private_exception_life
  type: boolean
- description: Private insurance coverage allowed for serious health conditions described by this field.
  name: private_exception_health
  type: string
- description: Private insurance coverage allowed for described fetal anomaly types.
  name: private_exception_fetal
  type: string
- description: If true, private insurance coverage allowed in cases of rape or incest.
  name: private_exception_rape_or_incest
  type: boolean
- description: If true, state has not restricted abortion coverage in ACA exchange plans.
  name: exchange_coverage_no_restrictions
  type: boolean
- description: If true, exchange plan coverage allowed when abortion is necessary to save pregnant person's life.
  name: exchange_exception_life
  type: boolean
- description: Exchange plan coverage allowed for health conditions described by this field.
  name: exchange_exception_health
  type: string
- description: Exchange plan coverage allowed for described fetal anomaly types.
  name: exchange_exception_fetal
  type: string
- description: If true, exchange plan coverage allowed in cases of rape or incest.
  name: exchange_exception_rape_or_incest
  type: boolean
- description: If true, state prohibits all exchange insurance coverage for abortion.
  name: exchange_forbids_coverage
  type: boolean
- description: If true, state uses Medicaid funds for medically necessary abortion determined by patient/provider.
  name: medicaid_coverage_provider_patient_decision
  type: boolean
- description: If true, Medicaid covers abortion necessary to save pregnant person's life (required by Hyde Amendment).
  name: medicaid_exception_life
  type: boolean
- description: Medicaid coverage for health conditions described by this field.
  name: medicaid_exception_health
  type: string
- description: Medicaid coverage for described fetal anomaly types.
  name: medicaid_exception_fetal
  type: string
- description: If true, Medicaid covers abortion in cases of rape or incest (required by Hyde Amendment).
  name: medicaid_exception_rape_or_incest
  type: boolean
- description: Date this policy record was last updated.
  name: Last Updated
  type: string
provider_name: Abortion Policy API
provider_slug: abortion-policy-api
schema_file: json-schema/insurance-coverage-schema.json
slug: insurance-coverage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/insurance-coverage-schema.json\",\n  \"title\": \"InsuranceCoverage\",\n  \"description\": \"Abortion insurance coverage restrictions covering Medicaid, private insurance, and ACA exchange plans for a US state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requires_coverage\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, state requires private health plans to cover abortion.\",\n      \"example\": false\n    },\n    \"private_coverage_no_restrictions\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, private insurance may cover abortion without restrictions.\",\n      \"example\": true\n    },\n    \"private_exception_life\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, private insurance coverage allowed when abortion is necessary\
  \ to save pregnant person's life.\",\n      \"example\": true\n    },\n    \"private_exception_health\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Private insurance coverage allowed for serious health conditions described by this field.\",\n      \"example\": \"Major Bodily Function\"\n    },\n    \"private_exception_fetal\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Private insurance coverage allowed for described fetal anomaly types.\",\n      \"example\": \"Lethal fetal anomaly\"\n    },\n    \"private_exception_rape_or_incest\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, private insurance coverage allowed in cases of rape or incest.\",\n      \"example\": true\n    },\n    \"exchange_coverage_no_restrictions\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, state has not restricted abortion coverage in ACA exchange plans.\",\n      \"example\": true\n    },\n\
  \    \"exchange_exception_life\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, exchange plan coverage allowed when abortion is necessary to save pregnant person's life.\",\n      \"example\": true\n    },\n    \"exchange_exception_health\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Exchange plan coverage allowed for health conditions described by this field.\",\n      \"example\": \"Physical\"\n    },\n    \"exchange_exception_fetal\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Exchange plan coverage allowed for described fetal anomaly types.\",\n      \"example\": \"Lethal fetal anomaly\"\n    },\n    \"exchange_exception_rape_or_incest\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, exchange plan coverage allowed in cases of rape or incest.\",\n      \"example\": true\n    },\n    \"exchange_forbids_coverage\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"If true, state prohibits all exchange insurance coverage for abortion.\",\n      \"example\": false\n    },\n    \"medicaid_coverage_provider_patient_decision\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, state uses Medicaid funds for medically necessary abortion determined by patient/provider.\",\n      \"example\": true\n    },\n    \"medicaid_exception_life\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, Medicaid covers abortion necessary to save pregnant person's life (required by Hyde Amendment).\",\n      \"example\": true\n    },\n    \"medicaid_exception_health\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Medicaid coverage for health conditions described by this field.\",\n      \"example\": \"Physical\"\n    },\n    \"medicaid_exception_fetal\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Medicaid coverage for described fetal anomaly types.\",\n \
  \     \"example\": \"Serious fetal anomaly\"\n    },\n    \"medicaid_exception_rape_or_incest\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, Medicaid covers abortion in cases of rape or incest (required by Hyde Amendment).\",\n      \"example\": true\n    },\n    \"Last Updated\": {\n      \"type\": \"string\",\n      \"description\": \"Date this policy record was last updated.\",\n      \"example\": \"2025-01-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/insurance-coverage-schema.json
tags:
- Abortion
- Policies
- Healthcare
- Government
title: InsuranceCoverage
---

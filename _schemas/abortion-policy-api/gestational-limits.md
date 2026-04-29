---
description: Abortion restrictions related to gestational limits (bans after certain weeks of pregnancy) for a US state or territory.
layout: schema
name: GestationalLimits
properties_list:
- description: Weeks since Last Menstrual Period (LMP) after which abortion is banned. Null means no gestational restriction. 99 means viability standard. 28 means third trimester ban. 0 means complete ban.
  name: banned_after_weeks_since_LMP
  type: integer
- description: If true, abortion is permitted when necessary to save the pregnant person's life.
  name: exception_life
  type: boolean
- description: Health exception type. "Physical" (excluding mental health), "Any" (may include mental health), or "Major Bodily Function" (substantial irreversible impairment).
  name: exception_health
  type: string
- description: Fetal anomaly exception type. "Serious fetal anomaly" or "Lethal fetal anomaly".
  name: exception_fetal
  type: string
- description: If true, exceptions may be granted in cases of rape or incest.
  name: exception_rape_or_incest
  type: boolean
- description: Date this policy record was last updated.
  name: Last Updated
  type: string
provider_name: Abortion Policy API
provider_slug: abortion-policy-api
schema_file: json-schema/gestational-limits-schema.json
slug: gestational-limits
source_filename: gestational-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/gestational-limits-schema.json\",\n  \"title\": \"GestationalLimits\",\n  \"description\": \"Abortion restrictions related to gestational limits (bans after certain weeks of pregnancy) for a US state or territory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"banned_after_weeks_since_LMP\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Weeks since Last Menstrual Period (LMP) after which abortion is banned. Null means no gestational restriction. 99 means viability standard. 28 means third trimester ban. 0 means complete ban.\",\n      \"example\": 24\n    },\n    \"exception_life\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, abortion is permitted when necessary to save the pregnant person's life.\",\n      \"example\": true\n \
  \   },\n    \"exception_health\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Health exception type. \\\"Physical\\\" (excluding mental health), \\\"Any\\\" (may include mental health), or \\\"Major Bodily Function\\\" (substantial irreversible impairment).\",\n      \"example\": \"Any\"\n    },\n    \"exception_fetal\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Fetal anomaly exception type. \\\"Serious fetal anomaly\\\" or \\\"Lethal fetal anomaly\\\".\",\n      \"example\": \"Serious fetal anomaly\"\n    },\n    \"exception_rape_or_incest\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, exceptions may be granted in cases of rape or incest.\",\n      \"example\": true\n    },\n    \"Last Updated\": {\n      \"type\": \"string\",\n      \"description\": \"Date this policy record was last updated.\",\n      \"example\": \"2025-01-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/gestational-limits-schema.json
tags:
- Abortion
- Policies
- Healthcare
- Government
title: GestationalLimits
---

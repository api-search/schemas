---
description: ''
layout: schema
name: HealthInfo
properties_list:
- description: ''
  name: country
  type: string
- description: ''
  name: vaccinations
  type: array
- description: ''
  name: healthRisks
  type: array
- description: ''
  name: drinkingWater
  type: string
- description: ''
  name: medicalFacilities
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/healthinfo.json
slug: healthinfo
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/healthinfo.json\",\n  \"title\": \"HealthInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"vaccinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"requirement\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"Required\",\n              \"Recommended\",\n              \"Optional\"\n            ]\n          }\n        }\n      }\n    },\n    \"healthRisks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"drinkingWater\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Safe\",\n        \"Unsafe\"\
  ,\n        \"Boil Advisories\"\n      ]\n    },\n    \"medicalFacilities\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Excellent\",\n        \"Good\",\n        \"Limited\",\n        \"Very Limited\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/healthinfo.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: HealthInfo
---

---
description: PlanInformation schema from Availity API
layout: schema
name: PlanInformation
properties_list:
- description: ''
  name: planName
  type: string
- description: ''
  name: groupName
  type: string
- description: ''
  name: groupNumber
  type: string
- description: ''
  name: planBeginDate
  type: string
- description: ''
  name: planEndDate
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-plan-information-schema.json
slug: eligibility-plan-information
source_filename: eligibility-plan-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-plan-information-schema.json\",\n  \"title\": \"PlanInformation\",\n  \"description\": \"PlanInformation schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"planName\": {\n      \"type\": \"string\"\n    },\n    \"groupName\": {\n      \"type\": \"string\"\n    },\n    \"groupNumber\": {\n      \"type\": \"string\"\n    },\n    \"planBeginDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"planEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-plan-information-schema.json
tags: []
title: PlanInformation
---

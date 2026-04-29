---
description: ''
layout: schema
name: AbsenceType
properties_list:
- description: The Workday ID of the absence type.
  name: id
  type: string
- description: A display descriptor for the absence type.
  name: descriptor
  type: string
- description: The category of the absence type (e.g., Vacation, Sick).
  name: absenceTypeCategory
  type: string
- description: The unit of measurement (e.g., Hours, Days).
  name: unit
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/absenceManagement-absence-type-schema.json
slug: absenceManagement-absence-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AbsenceType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the absence type.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the absence type.\"\n    },\n    \"absenceTypeCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the absence type (e.g., Vacation, Sick).\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measurement (e.g., Hours, Days).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/absenceManagement-absence-type-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: AbsenceType
---

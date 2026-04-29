---
description: Abortion waiting period restrictions in a US state, covering mandatory time between counseling and abortion care.
layout: schema
name: WaitingPeriods
properties_list:
- description: Hours a person must wait between receiving state-mandated counseling and obtaining abortion. Null means no waiting period.
  name: waiting_period_hours
  type: integer
- description: 1=counseling required by state; 2=counseling must be at the facility, requiring two clinic trips.
  name: counseling_visits
  type: integer
- description: Conditions under which waiting period may be waived.
  name: exception_health
  type: string
- description: Additional notes on unusual waiting period policies.
  name: waiting_period_notes
  type: string
- description: Conditions under which counseling requirement can be waived.
  name: counseling_waived_condition
  type: string
- description: Date this policy record was last updated.
  name: Last Updated
  type: string
provider_name: Abortion Policy API
provider_slug: abortion-policy-api
schema_file: json-schema/waiting-periods-schema.json
slug: waiting-periods
source_filename: waiting-periods-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/waiting-periods-schema.json\",\n  \"title\": \"WaitingPeriods\",\n  \"description\": \"Abortion waiting period restrictions in a US state, covering mandatory time between counseling and abortion care.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"waiting_period_hours\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Hours a person must wait between receiving state-mandated counseling and obtaining abortion. Null means no waiting period.\",\n      \"example\": 24\n    },\n    \"counseling_visits\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"1=counseling required by state; 2=counseling must be at the facility, requiring two clinic trips.\",\n      \"example\": 1\n    },\n    \"exception_health\": {\n      \"type\"\
  : \"string\",\n      \"nullable\": true,\n      \"description\": \"Conditions under which waiting period may be waived.\",\n      \"example\": \"Medical emergency\"\n    },\n    \"waiting_period_notes\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Additional notes on unusual waiting period policies.\",\n      \"example\": \"Waiting period waived in medical emergencies.\"\n    },\n    \"counseling_waived_condition\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Conditions under which counseling requirement can be waived.\",\n      \"example\": \"Medical emergency\"\n    },\n    \"Last Updated\": {\n      \"type\": \"string\",\n      \"description\": \"Date this policy record was last updated.\",\n      \"example\": \"2025-01-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/json-schema/waiting-periods-schema.json
tags:
- Abortion
- Policies
- Healthcare
- Government
title: WaitingPeriods
---

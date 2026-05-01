---
description: Status and lifecycle metadata for a Veteran benefits claim.
layout: schema
name: VA Benefits Claim
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Department of Veterans Affairs (VA)
provider_slug: department-of-veterans-affairs
schema_file: json-schema/va-claim-schema.json
slug: va-claim
source_filename: va-claim-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-veterans-affairs/schemas/claim.json\",\n  \"title\": \"VA Benefits Claim\",\n  \"description\": \"Status and lifecycle metadata for a Veteran benefits claim.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"attributes\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"type\": { \"type\": \"string\", \"const\": \"claim\" },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"baseEndProductCode\": { \"type\": [\"string\", \"null\"] },\n        \"claimDate\": { \"type\": [\"string\", \"null\"], \"format\": \"date\" },\n        \"claimType\": { \"type\": [\"string\", \"null\"] },\n        \"claimPhaseDates\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"phaseChangeDate\": { \"type\": [\"string\", \"null\"], \"format\": \"date\" },\n            \"currentPhaseBack\"\
  : { \"type\": \"boolean\" },\n            \"latestPhaseType\": { \"type\": [\"string\", \"null\"] }\n          }\n        },\n        \"decisionLetterSent\": { \"type\": \"boolean\" },\n        \"developmentLetterSent\": { \"type\": \"boolean\" },\n        \"documentsNeeded\": { \"type\": \"boolean\" },\n        \"endProductCode\": { \"type\": [\"string\", \"null\"] },\n        \"evidenceWaiverSubmitted5103\": { \"type\": \"boolean\" },\n        \"lighthouseId\": { \"type\": [\"string\", \"null\"] },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"PENDING\",\n            \"CLAIM_RECEIVED\",\n            \"INITIAL_REVIEW\",\n            \"EVIDENCE_GATHERING_REVIEW_DECISION\",\n            \"PREPARATION_FOR_NOTIFICATION\",\n            \"COMPLETE\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-veterans-affairs/refs/heads/main/json-schema/va-claim-schema.json
tags:
- Federal Government
- Healthcare
- Veterans
title: VA Benefits Claim
---

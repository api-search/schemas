---
description: UnderwritingSubmissionResponse schema from ACORD NGDS API
layout: schema
name: UnderwritingSubmissionResponse
properties_list:
- description: ''
  name: submissionId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: submittedAt
  type: string
- description: ''
  name: notes
  type: string
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-underwriting-submission-response-schema.json
slug: ngds-underwriting-submission-response
source_filename: ngds-underwriting-submission-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-underwriting-submission-response-schema.json\",\n  \"title\": \"UnderwritingSubmissionResponse\",\n  \"description\": \"UnderwritingSubmissionResponse schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"submissionId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Received\",\n        \"UnderReview\",\n        \"Approved\",\n        \"Declined\",\n        \"RequiresMoreInfo\"\n      ]\n    },\n    \"submittedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"notes\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-underwriting-submission-response-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: UnderwritingSubmissionResponse
---

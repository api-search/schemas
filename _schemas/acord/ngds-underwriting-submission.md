---
description: UnderwritingSubmission schema from ACORD NGDS API
layout: schema
name: UnderwritingSubmission
properties_list:
- description: ''
  name: lineOfBusiness
  type: string
- description: ''
  name: applicant
  type: object
- description: ''
  name: requestedEffectiveDate
  type: string
- description: ''
  name: requestedExpirationDate
  type: string
- description: ''
  name: riskDetails
  type: object
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-underwriting-submission-schema.json
slug: ngds-underwriting-submission
source_filename: ngds-underwriting-submission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-underwriting-submission-schema.json\",\n  \"title\": \"UnderwritingSubmission\",\n  \"description\": \"UnderwritingSubmission schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineOfBusiness\": {\n      \"type\": \"string\"\n    },\n    \"applicant\": {\n      \"$ref\": \"#/components/schemas/PartyRequest\"\n    },\n    \"requestedEffectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"requestedExpirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"riskDetails\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\n    \"lineOfBusiness\",\n    \"applicant\",\n    \"requestedEffectiveDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-underwriting-submission-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: UnderwritingSubmission
---

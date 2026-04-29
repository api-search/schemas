---
description: EligibilityResponse schema from Availity API
layout: schema
name: EligibilityResponse
properties_list:
- description: Availity transaction ID
  name: id
  type: string
- description: ''
  name: controlNumber
  type: string
- description: ''
  name: requestedDate
  type: string
- description: ''
  name: serviceDate
  type: string
- description: ''
  name: subscriber
  type: object
- description: ''
  name: payer
  type: object
- description: ''
  name: coverages
  type: array
- description: ''
  name: planInformation
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-eligibility-response-schema.json
slug: eligibility-eligibility-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-eligibility-response-schema.json\",\n  \"title\": \"EligibilityResponse\",\n  \"description\": \"EligibilityResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Availity transaction ID\"\n    },\n    \"controlNumber\": {\n      \"type\": \"string\"\n    },\n    \"requestedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"serviceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"subscriber\": {\n      \"$ref\": \"#/components/schemas/SubscriberInfo\"\n    },\n    \"payer\": {\n      \"$ref\": \"#/components/schemas/PayerInfo\"\n    },\n    \"coverages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Coverage\"\
  \n      }\n    },\n    \"planInformation\": {\n      \"$ref\": \"#/components/schemas/PlanInformation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-eligibility-response-schema.json
tags: []
title: EligibilityResponse
---

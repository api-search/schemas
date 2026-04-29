---
description: SearchBy276Request schema from Availity API
layout: schema
name: SearchBy276Request
properties_list:
- description: ''
  name: payerId
  type: string
- description: ''
  name: patientLastName
  type: string
- description: ''
  name: patientFirstName
  type: string
- description: ''
  name: patientBirthDate
  type: string
- description: ''
  name: fromDate
  type: string
- description: ''
  name: toDate
  type: string
- description: ''
  name: providerLastName
  type: string
- description: ''
  name: patientSameAsSubscriber
  type: boolean
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-search-by276-request-schema.json
slug: claim-status-search-by276-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-search-by276-request-schema.json\",\n  \"title\": \"SearchBy276Request\",\n  \"description\": \"SearchBy276Request schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"patientLastName\",\n    \"patientFirstName\",\n    \"patientBirthDate\",\n    \"fromDate\",\n    \"toDate\",\n    \"providerLastName\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"example\": \"BCBS001\"\n    },\n    \"patientLastName\": {\n      \"type\": \"string\",\n      \"example\": \"Smith\"\n    },\n    \"patientFirstName\": {\n      \"type\": \"string\",\n      \"example\": \"Jane\"\n    },\n    \"patientBirthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"1980-01-15\"\n    },\n    \"fromDate\": {\n \
  \     \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-01-01\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-12-31\"\n    },\n    \"providerLastName\": {\n      \"type\": \"string\",\n      \"example\": \"Johnson\"\n    },\n    \"patientSameAsSubscriber\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-search-by276-request-schema.json
tags: []
title: SearchBy276Request
---

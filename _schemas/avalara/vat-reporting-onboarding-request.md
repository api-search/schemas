---
description: OnboardingRequest schema from Avalara API
layout: schema
name: OnboardingRequest
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: countries
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-onboarding-request-schema.json
slug: vat-reporting-onboarding-request
source_filename: vat-reporting-onboarding-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-onboarding-request-schema.json\",\n  \"title\": \"OnboardingRequest\",\n  \"description\": \"OnboardingRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"companyId\",\n    \"countries\"\n  ],\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"countries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"countryCode\": {\n            \"type\": \"string\"\n          },\n          \"vatRegistrationNumber\": {\n            \"type\": \"string\"\n          },\n          \"filingFrequency\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"Monthly\",\n              \"Quarterly\"\
  ,\n              \"Annual\"\n            ]\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-onboarding-request-schema.json
tags:
- Taxes
title: OnboardingRequest
---

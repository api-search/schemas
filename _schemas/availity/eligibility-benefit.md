---
description: Benefit schema from Availity API
layout: schema
name: Benefit
properties_list:
- description: X12 benefit information code
  name: code
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: coverageLevel
  type: string
- description: ''
  name: benefitAmount
  type: object
- description: ''
  name: benefitPercent
  type: number
- description: ''
  name: inPlanNetworkIndicator
  type: string
- description: Benefit period (e.g., Calendar Year, Plan Year, Lifetime)
  name: timeQualifier
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-benefit-schema.json
slug: eligibility-benefit
source_filename: eligibility-benefit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-benefit-schema.json\",\n  \"title\": \"Benefit\",\n  \"description\": \"Benefit schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"X12 benefit information code\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"coverageLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INDIVIDUAL\",\n        \"FAMILY\",\n        \"EMPLOYEE\",\n        \"EMPLOYEE_AND_SPOUSE\"\n      ]\n    },\n    \"benefitAmount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"number\"\n        },\n        \"currency\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"benefitPercent\": {\n      \"type\": \"number\",\n      \"\
  minimum\": 0,\n      \"maximum\": 100\n    },\n    \"inPlanNetworkIndicator\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Y\",\n        \"N\",\n        \"W\"\n      ]\n    },\n    \"timeQualifier\": {\n      \"type\": \"string\",\n      \"description\": \"Benefit period (e.g., Calendar Year, Plan Year, Lifetime)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-benefit-schema.json
tags: []
title: Benefit
---

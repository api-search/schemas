---
description: ''
layout: schema
name: EligibleEnrollmentPeriod
properties_list:
- description: ''
  name: isEnrollmentRequired
  type: boolean
- description: ''
  name: enrollmentStartDate
  type: string
- description: ''
  name: enrollmentEndDate
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-eligible-enrollment-period-schema.json
slug: salesforce-eligible-enrollment-period
source_filename: salesforce-eligible-enrollment-period-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"isEnrollmentRequired\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"enrollmentStartDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"enrollmentEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"isEnrollmentRequired\",\n    \"enrollmentStartDate\",\n    \"enrollmentEndDate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EligibleEnrollmentPeriod\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-eligible-enrollment-period-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: EligibleEnrollmentPeriod
---

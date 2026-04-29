---
description: ''
layout: schema
name: UpdateMemberDetailsRequest
properties_list:
- description: ''
  name: processParameters
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update-member-details-request-schema.json
slug: salesforce-update-member-details-request
source_filename: salesforce-update-member-details-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"processParameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"MemberId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"MembershipNumber\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Email\": {\n            \"type\": \"string\",\n            \"example\": \"user@example.com\"\n          },\n          \"EnrollmentDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"LastName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"MemberId\",\n          \"MembershipNumber\",\n          \"Email\",\n          \"EnrollmentDate\"\
  ,\n          \"LastName\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"processParameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateMemberDetailsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update-member-details-request-schema.json
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
title: UpdateMemberDetailsRequest
---

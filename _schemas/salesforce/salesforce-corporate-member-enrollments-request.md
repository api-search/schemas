---
description: ''
layout: schema
name: CorporateMemberEnrollmentsRequest
properties_list:
- description: ''
  name: enrollmentDate
  type: string
- description: ''
  name: membershipNumber
  type: string
- description: ''
  name: associatedAccountDetails
  type: object
- description: ''
  name: memberStatus
  type: string
- description: ''
  name: createTransactionJournals
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-corporate-member-enrollments-request-schema.json
slug: salesforce-corporate-member-enrollments-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrollmentDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"membershipNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"associatedAccountDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"website\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"allowDuplicateRecords\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"phone\",\n        \"website\",\n        \"allowDuplicateRecords\"\n      ]\n    },\n    \"memberStatus\": {\n      \"type\": \"\
  string\",\n      \"example\": \"example_value\"\n    },\n    \"createTransactionJournals\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"enrollmentDate\",\n    \"membershipNumber\",\n    \"associatedAccountDetails\",\n    \"memberStatus\",\n    \"createTransactionJournals\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CorporateMemberEnrollmentsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-corporate-member-enrollments-request-schema.json
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
title: CorporateMemberEnrollmentsRequest
---

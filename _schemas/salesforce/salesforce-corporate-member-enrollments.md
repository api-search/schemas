---
description: ''
layout: schema
name: CorporateMemberEnrollments
properties_list:
- description: ''
  name: accountId
  type: string
- description: ''
  name: loyaltyProgramMemberId
  type: string
- description: ''
  name: loyaltyProgramName
  type: string
- description: ''
  name: membershipNumber
  type: string
- description: ''
  name: transactionJournals
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-corporate-member-enrollments-schema.json
slug: salesforce-corporate-member-enrollments
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"loyaltyProgramMemberId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"loyaltyProgramName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"membershipNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"activityDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"journalSubType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"journalType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\
  \n          },\n          \"loyaltyProgram\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"loyaltyProgramMember\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"referredMember\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"transactionJournalId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"activityDate\",\n          \"journalSubType\",\n          \"journalType\",\n          \"loyaltyProgram\",\n          \"loyaltyProgramMember\",\n          \"referredMember\",\n          \"status\",\n          \"transactionJournalId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"accountId\"\
  ,\n    \"loyaltyProgramMemberId\",\n    \"loyaltyProgramName\",\n    \"membershipNumber\",\n    \"transactionJournals\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CorporateMemberEnrollments\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-corporate-member-enrollments-schema.json
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
title: CorporateMemberEnrollments
---

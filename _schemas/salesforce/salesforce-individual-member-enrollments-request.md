---
description: ''
layout: schema
name: IndividualMemberEnrollmentsRequest
properties_list:
- description: ''
  name: enrollmentDate
  type: string
- description: ''
  name: membershipNumber
  type: string
- description: ''
  name: associatedContactDetails
  type: object
- description: ''
  name: memberStatus
  type: string
- description: ''
  name: createTransactionJournals
  type: string
- description: ''
  name: transactionJournalStatementFrequency
  type: string
- description: ''
  name: transactionJournalStatementMethod
  type: string
- description: ''
  name: enrollmentChannel
  type: string
- description: ''
  name: canReceivePromotions
  type: string
- description: ''
  name: canReceivePartnerPromotions
  type: string
- description: ''
  name: membershipEndDate
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-individual-member-enrollments-request-schema.json
slug: salesforce-individual-member-enrollments-request
source_filename: salesforce-individual-member-enrollments-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrollmentDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"membershipNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"associatedContactDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n        },\n        \"allowDuplicateRecords\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"firstName\",\n        \"lastName\",\n        \"email\",\n        \"allowDuplicateRecords\"\n      ]\n    },\n    \"memberStatus\": {\n   \
  \   \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"createTransactionJournals\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournalStatementFrequency\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournalStatementMethod\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"enrollmentChannel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"canReceivePromotions\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"canReceivePartnerPromotions\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"membershipEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"enrollmentDate\",\n    \"membershipNumber\",\n    \"associatedContactDetails\",\n    \"memberStatus\",\n \
  \   \"createTransactionJournals\",\n    \"transactionJournalStatementFrequency\",\n    \"transactionJournalStatementMethod\",\n    \"enrollmentChannel\",\n    \"canReceivePromotions\",\n    \"canReceivePartnerPromotions\",\n    \"membershipEndDate\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndividualMemberEnrollmentsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-individual-member-enrollments-request-schema.json
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
title: IndividualMemberEnrollmentsRequest
---

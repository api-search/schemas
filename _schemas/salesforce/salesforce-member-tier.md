---
description: ''
layout: schema
name: MemberTier
properties_list:
- description: ''
  name: additionalLoyaltyMemberTierFields
  type: object
- description: ''
  name: areTierBenefitsAssigned
  type: boolean
- description: ''
  name: loyaltyMemberTierId
  type: string
- description: ''
  name: loyaltyMemberTierName
  type: string
- description: ''
  name: tierChangeReason
  type: '[''string'', ''null'']'
- description: ''
  name: tierChangeReasonType
  type: '[''string'', ''null'']'
- description: ''
  name: tierEffectiveDate
  type: string
- description: ''
  name: tierExpirationDate
  type: '[''string'', ''null'']'
- description: ''
  name: tierGroupId
  type: string
- description: ''
  name: tierGroupName
  type: '[''string'', ''null'']'
- description: ''
  name: tierId
  type: string
- description: ''
  name: tierSequenceNumber
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-member-tier-schema.json
slug: salesforce-member-tier
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalLoyaltyMemberTierFields\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"areTierBenefitsAssigned\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"loyaltyMemberTierId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"loyaltyMemberTierName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"tierChangeReason\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"tierChangeReasonType\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"tierEffectiveDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"tierExpirationDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"tierGroupId\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"500123\"\n    },\n    \"tierGroupName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"tierId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"tierSequenceNumber\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"additionalLoyaltyMemberTierFields\",\n    \"areTierBenefitsAssigned\",\n    \"loyaltyMemberTierId\",\n    \"loyaltyMemberTierName\",\n    \"tierChangeReason\",\n    \"tierChangeReasonType\",\n    \"tierEffectiveDate\",\n    \"tierExpirationDate\",\n    \"tierGroupId\",\n    \"tierGroupName\",\n    \"tierId\",\n    \"tierSequenceNumber\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemberTier\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-member-tier-schema.json
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
title: MemberTier
---

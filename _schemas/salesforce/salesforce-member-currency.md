---
description: ''
layout: schema
name: MemberCurrency
properties_list:
- description: ''
  name: additionalLoyaltyMemberCurrencyFields
  type: object
- description: ''
  name: escrowPointsBalance
  type: integer
- description: ''
  name: expirablePoints
  type: integer
- description: ''
  name: lastAccrualProcessedDate
  type: '[''string'', ''null'']'
- description: ''
  name: lastEscrowProcessedDate
  type: '[''string'', ''null'']'
- description: ''
  name: lastExpirationProcessRunDate
  type: '[''string'', ''null'']'
- description: ''
  name: lastPointsAggregationDate
  type: '[''string'', ''null'']'
- description: ''
  name: lastPointsResetDate
  type: '[''string'', ''null'']'
- description: ''
  name: loyaltyMemberCurrencyName
  type: string
- description: ''
  name: loyaltyProgramCurrencyId
  type: string
- description: ''
  name: loyaltyProgramCurrencyName
  type: '[''string'', ''null'']'
- description: ''
  name: memberCurrencyId
  type: string
- description: ''
  name: nextQualifyingPointsResetDate
  type: string
- description: ''
  name: pointsBalance
  type: integer
- description: ''
  name: qualifyingPointsBalanceBeforeReset
  type: integer
- description: ''
  name: totalEscrowPointsAccrued
  type: integer
- description: ''
  name: totalEscrowRolloverPoints
  type: integer
- description: ''
  name: totalPointsAccrued
  type: integer
- description: ''
  name: totalPointsExpired
  type: integer
- description: ''
  name: totalPointsRedeemed
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-member-currency-schema.json
slug: salesforce-member-currency
source_filename: salesforce-member-currency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalLoyaltyMemberCurrencyFields\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Level_Before_Reset__c\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"Level_Before_Reset__c\"\n      ]\n    },\n    \"escrowPointsBalance\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"expirablePoints\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"lastAccrualProcessedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastEscrowProcessedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastExpirationProcessRunDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastPointsAggregationDate\": {\n      \"type\": \"\
  ['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastPointsResetDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"loyaltyMemberCurrencyName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"loyaltyProgramCurrencyId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"loyaltyProgramCurrencyName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"memberCurrencyId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"nextQualifyingPointsResetDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"pointsBalance\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"qualifyingPointsBalanceBeforeReset\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"totalEscrowPointsAccrued\": {\n      \"type\": \"integer\"\
  ,\n      \"example\": 42\n    },\n    \"totalEscrowRolloverPoints\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"totalPointsAccrued\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"totalPointsExpired\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"totalPointsRedeemed\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"additionalLoyaltyMemberCurrencyFields\",\n    \"escrowPointsBalance\",\n    \"expirablePoints\",\n    \"lastAccrualProcessedDate\",\n    \"lastEscrowProcessedDate\",\n    \"lastExpirationProcessRunDate\",\n    \"lastPointsAggregationDate\",\n    \"lastPointsResetDate\",\n    \"loyaltyMemberCurrencyName\",\n    \"loyaltyProgramCurrencyId\",\n    \"loyaltyProgramCurrencyName\",\n    \"memberCurrencyId\",\n    \"nextQualifyingPointsResetDate\",\n    \"pointsBalance\",\n    \"qualifyingPointsBalanceBeforeReset\",\n    \"totalEscrowPointsAccrued\",\n    \"totalEscrowRolloverPoints\"\
  ,\n    \"totalPointsAccrued\",\n    \"totalPointsExpired\",\n    \"totalPointsRedeemed\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemberCurrency\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-member-currency-schema.json
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
title: MemberCurrency
---

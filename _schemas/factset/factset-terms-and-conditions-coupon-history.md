---
description: Coupon History for a Fixed Income security.
layout: schema
name: couponHistory
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Coupon Accrual Date
  name: date
  type: string
- description: Coupon Basket Flag
  name: couponBasketFlag
  type: boolean
- description: Effective Payment Date
  name: couponEffPmtDate
  type: string
- description: Coupon Formula
  name: couponFormula
  type: string
- description: First Coupon Reset Date
  name: couponInitResetDate
  type: string
- description: Coupon Reset Frequency
  name: couponResetFreq
  type: string
- description: Coupon Link
  name: couponLink
  type: string
- description: Margin
  name: couponMargin
  type: number
- description: Coupon Minimum-Floating Rate
  name: couponMinFloatRate
  type: number
- description: Coupon Structure Sub Code
  name: couponStructSubCode
  type: string
- description: Coupon Type
  name: couponTypeStruct
  type: string
- description: Variable Coupon Payments
  name: couponVarPmtFlag
  type: boolean
- description: Underlying Index
  name: underlyingIndex
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-coupon-history-schema.json
slug: factset-terms-and-conditions-coupon-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"couponHistory\",\n  \"type\": \"object\",\n  \"description\": \"Coupon History for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Accrual Date\"\n    },\n    \"couponBasketFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Coupon Basket Flag\"\n    },\n    \"couponEffPmtDate\": {\n      \"type\": \"string\",\n      \"description\": \"Effective Payment Date\"\n    },\n    \"couponFormula\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Formula\"\n    },\n    \"couponInitResetDate\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"First Coupon Reset Date\"\n    },\n    \"couponResetFreq\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Reset Frequency\"\n    },\n    \"couponLink\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Link\"\n    },\n    \"couponMargin\": {\n      \"type\": \"number\",\n      \"description\": \"Margin\"\n    },\n    \"couponMinFloatRate\": {\n      \"type\": \"number\",\n      \"description\": \"Coupon Minimum-Floating Rate\"\n    },\n    \"couponStructSubCode\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Structure Sub Code\"\n    },\n    \"couponTypeStruct\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Type\"\n    },\n    \"couponVarPmtFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Variable Coupon Payments\"\n    },\n    \"underlyingIndex\": {\n      \"type\": \"string\",\n      \"description\": \"Underlying Index\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-coupon-history-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: couponHistory
---

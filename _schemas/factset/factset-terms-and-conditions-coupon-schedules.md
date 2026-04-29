---
description: Coupon Schedules for a Fixed Income security.
layout: schema
name: couponSchedules
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Coupon Effective Date
  name: couponEffDate
  type: string
- description: Coupon Rate
  name: couponRate
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-coupon-schedules-schema.json
slug: factset-terms-and-conditions-coupon-schedules
source_filename: factset-terms-and-conditions-coupon-schedules-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"couponSchedules\",\n  \"type\": \"object\",\n  \"description\": \"Coupon Schedules for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"couponEffDate\": {\n      \"type\": \"string\",\n      \"description\": \"Coupon Effective Date\"\n    },\n    \"couponRate\": {\n      \"type\": \"number\",\n      \"description\": \"Coupon Rate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-coupon-schedules-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: couponSchedules
---

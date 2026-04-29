---
description: Request to report partner miles for a Mileage Plan member
layout: schema
name: PartnerMilesRequest
properties_list:
- description: Mileage Plan member number
  name: memberId
  type: string
- description: Registered partner identifier
  name: partnerId
  type: string
- description: Type of partner activity
  name: activityType
  type: string
- description: Date of partner activity
  name: activityDate
  type: string
- description: Transaction amount in partner currency
  name: activityAmount
  type: number
- description: Currency code
  name: currency
  type: string
- description: Miles to credit
  name: miles
  type: integer
- description: Partner activity reference number
  name: referenceId
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-mileage-plan-partner-miles-request-schema.json
slug: alaska-air-mileage-plan-partner-miles-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-partner-miles-request-schema.json\",\n  \"title\": \"PartnerMilesRequest\",\n  \"description\": \"Request to report partner miles for a Mileage Plan member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memberId\": {\n      \"type\": \"string\",\n      \"description\": \"Mileage Plan member number\",\n      \"example\": \"12345678\"\n    },\n    \"partnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Registered partner identifier\",\n      \"example\": \"MARRIOTT\"\n    },\n    \"activityType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of partner activity\",\n      \"enum\": [\n        \"hotel_stay\",\n        \"car_rental\",\n        \"retail\",\n        \"flight\",\n        \"dining\"\n      ],\n      \"example\": \"hotel_stay\"\n    },\n\
  \    \"activityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of partner activity\",\n      \"example\": \"2026-04-15\"\n    },\n    \"activityAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount in partner currency\",\n      \"example\": 285.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"USD\"\n    },\n    \"miles\": {\n      \"type\": \"integer\",\n      \"description\": \"Miles to credit\",\n      \"example\": 500\n    },\n    \"referenceId\": {\n      \"type\": \"string\",\n      \"description\": \"Partner activity reference number\",\n      \"example\": \"RES-123456\"\n    }\n  },\n  \"required\": [\n    \"memberId\",\n    \"partnerId\",\n    \"activityType\",\n    \"activityDate\",\n    \"miles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-partner-miles-request-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: PartnerMilesRequest
---

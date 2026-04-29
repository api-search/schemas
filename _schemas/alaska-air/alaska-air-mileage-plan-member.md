---
description: Alaska Airlines Mileage Plan member
layout: schema
name: Member
properties_list:
- description: Mileage Plan member number
  name: memberId
  type: string
- description: Member first name
  name: firstName
  type: string
- description: Member last name
  name: lastName
  type: string
- description: Member email address
  name: email
  type: string
- description: Current MVP tier status
  name: tier
  type: string
- description: Current available mile balance
  name: mileBalance
  type: integer
- description: Miles earned toward tier qualification
  name: tierMiles
  type: integer
- description: Membership start date
  name: memberSince
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-mileage-plan-member-schema.json
slug: alaska-air-mileage-plan-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-member-schema.json\",\n  \"title\": \"Member\",\n  \"description\": \"Alaska Airlines Mileage Plan member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memberId\": {\n      \"type\": \"string\",\n      \"description\": \"Mileage Plan member number\",\n      \"example\": \"12345678\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"Member first name\",\n      \"example\": \"Jane\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Member last name\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Member email address\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"tier\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Current MVP tier status\",\n      \"enum\": [\n        \"Member\",\n        \"MVP\",\n        \"MVP Gold\",\n        \"MVP Gold 75K\"\n      ],\n      \"example\": \"MVP Gold 75K\"\n    },\n    \"mileBalance\": {\n      \"type\": \"integer\",\n      \"description\": \"Current available mile balance\",\n      \"example\": 125000\n    },\n    \"tierMiles\": {\n      \"type\": \"integer\",\n      \"description\": \"Miles earned toward tier qualification\",\n      \"example\": 78500\n    },\n    \"memberSince\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Membership start date\",\n      \"example\": \"2018-03-15\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-member-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Member
---

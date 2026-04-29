---
description: Schema for a BJ's Wholesale Club membership record
layout: schema
name: BJS Membership
properties_list:
- description: BJ's membership card number
  name: membershipNumber
  type: string
- description: Current membership status
  name: status
  type: string
- description: Membership tier level
  name: tier
  type: string
- description: Membership expiration date
  name: expirationDate
  type: string
- description: Name of the primary account holder
  name: primaryMember
  type: string
provider_name: BJ's Wholesale Club
provider_slug: bjs-wholesale-club
schema_file: json-schema/bjs-membership-schema.json
slug: bjs-membership
source_filename: bjs-membership-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/main/json-schema/bjs-membership-schema.json\",\n  \"title\": \"BJS Membership\",\n  \"description\": \"Schema for a BJ's Wholesale Club membership record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"membershipNumber\": {\n      \"type\": \"string\",\n      \"description\": \"BJ's membership card number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"expired\", \"suspended\"],\n      \"description\": \"Current membership status\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"enum\": [\"inner_circle\", \"inner_circle_gold\", \"business\"],\n      \"description\": \"Membership tier level\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Membership expiration date\"\n    },\n    \"primaryMember\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the primary account holder\"\n    }\n  },\n  \"required\": [\"membershipNumber\", \"status\", \"tier\", \"expirationDate\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bjs-wholesale-club/refs/heads/main/json-schema/bjs-membership-schema.json
tags:
- Ecommerce
- Membership
- Retail
- Wholesale
title: BJS Membership
---

---
description: Player profile and account information.
layout: schema
name: PlayerInfoResponse
properties_list:
- description: Whether the request succeeded.
  name: success
  type: boolean
- description: Unique player user ID.
  name: userId
  type: string
- description: Player's username.
  name: userName
  type: string
- description: Player's first name.
  name: firstName
  type: string
- description: Player's last name.
  name: lastName
  type: string
- description: Player's email address.
  name: email
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: countryCode
  type: string
- description: ISO 4217 currency code for the player's account.
  name: currency
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-player-info-response-schema.json
slug: wallet-api-player-info-response
source_filename: wallet-api-player-info-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-player-info-response-schema.json\",\n  \"title\": \"PlayerInfoResponse\",\n  \"description\": \"Player profile and account information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request succeeded.\",\n      \"example\": true\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique player user ID.\",\n      \"example\": \"player-500123\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Player's username.\",\n      \"example\": \"jsmith\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"Player's first name.\",\n      \"example\": \"Jane\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Player's last name.\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Player's email address.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\",\n      \"example\": \"US\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the player's account.\",\n      \"example\": \"USD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-player-info-response-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: PlayerInfoResponse
---

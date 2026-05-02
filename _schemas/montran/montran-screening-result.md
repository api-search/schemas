---
description: The result of a sanctions screening operation performed by Montran's Enhanced Filtering System (EFS). Contains match information from screening against compliance lists such as OFAC, EU, OFSI, Lloyds MIU, and UN sanctions lists.
layout: schema
name: Montran Screening Result
properties_list:
- description: Unique screening operation identifier
  name: screeningId
  type: string
- description: Overall screening result
  name: result
  type: string
- description: Type of screening performed
  name: screeningType
  type: string
- description: Screening channel used
  name: channelId
  type: string
- description: Number of matches found
  name: matchCount
  type: integer
- description: Individual match details
  name: matches
  type: array
- description: Reference to the screened transaction
  name: transactionReference
  type: string
- description: Format of the screened message
  name: messageFormat
  type: string
- description: Timestamp when screening was performed
  name: screenedAt
  type: string
- description: Screening processing time in milliseconds
  name: latencyMs
  type: integer
provider_name: Montran
provider_slug: montran
schema_file: json-schema/montran-screening-result-schema.json
slug: montran-screening-result
source_filename: montran-screening-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.montran.com/schemas/screening-result.json\",\n  \"title\": \"Montran Screening Result\",\n  \"description\": \"The result of a sanctions screening operation performed by Montran's Enhanced Filtering System (EFS). Contains match information from screening against compliance lists such as OFAC, EU, OFSI, Lloyds MIU, and UN sanctions lists.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"screeningId\",\n    \"result\",\n    \"screenedAt\"\n  ],\n  \"properties\": {\n    \"screeningId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique screening operation identifier\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"Overall screening result\",\n      \"enum\": [\n        \"PASS\",\n        \"HIT\",\n        \"POSSIBLE_HIT\"\n      ]\n    },\n    \"screeningType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of screening\
  \ performed\",\n      \"enum\": [\n        \"transaction\",\n        \"entity\",\n        \"batch\"\n      ]\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"Screening channel used\"\n    },\n    \"matchCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of matches found\",\n      \"minimum\": 0\n    },\n    \"matches\": {\n      \"type\": \"array\",\n      \"description\": \"Individual match details\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ScreeningMatch\"\n      }\n    },\n    \"transactionReference\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to the screened transaction\"\n    },\n    \"messageFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Format of the screened message\",\n      \"enum\": [\n        \"ISO20022\",\n        \"SWIFT_FIN\",\n        \"ISO8583\",\n        \"NACHA\",\n        \"PROPRIETARY\"\n      ]\n    },\n    \"screenedAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when screening was performed\"\n    },\n    \"latencyMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Screening processing time in milliseconds\",\n      \"minimum\": 0\n    }\n  },\n  \"$defs\": {\n    \"ScreeningMatch\": {\n      \"type\": \"object\",\n      \"description\": \"Individual match against a sanctions or compliance list entry\",\n      \"properties\": {\n        \"matchId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique match identifier\"\n        },\n        \"matchedField\": {\n          \"type\": \"string\",\n          \"description\": \"Transaction field that triggered the match\",\n          \"enum\": [\n            \"debtorName\",\n            \"creditorName\",\n            \"debtorAddress\",\n            \"creditorAddress\",\n            \"debtorCountry\",\n            \"creditorCountry\",\n            \"remittanceInformation\"\n          ]\n        },\n\
  \        \"matchedValue\": {\n          \"type\": \"string\",\n          \"description\": \"Value from the transaction that matched\"\n        },\n        \"listSource\": {\n          \"type\": \"string\",\n          \"description\": \"Source of the compliance list\",\n          \"enum\": [\n            \"OFAC\",\n            \"EU\",\n            \"OFSI\",\n            \"UN\",\n            \"LLOYDS_MIU\",\n            \"CUSTOM\"\n          ]\n        },\n        \"listName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the compliance list\"\n        },\n        \"listEntryId\": {\n          \"type\": \"string\",\n          \"description\": \"Entry identifier in the compliance list\"\n        },\n        \"listedName\": {\n          \"type\": \"string\",\n          \"description\": \"Name as it appears on the sanctions list\"\n        },\n        \"matchScore\": {\n          \"type\": \"number\",\n          \"description\": \"Match confidence score (0-100)\"\
  ,\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"matchType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of matching algorithm that produced the match\",\n          \"enum\": [\n            \"EXACT\",\n            \"FUZZY\",\n            \"PHONETIC\",\n            \"PARTIAL\"\n          ]\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"description\": \"Match severity level\",\n          \"enum\": [\n            \"high\",\n            \"medium\",\n            \"low\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/json-schema/montran-screening-result-schema.json
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
title: Montran Screening Result
---

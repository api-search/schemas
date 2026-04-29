---
description: ''
layout: schema
name: TermAndCondition
properties_list:
- description: This defines what type of modification is concerned in this rule.
  name: category
  type: string
- description: ''
  name: circumstances
  type: string
- description: ''
  name: notApplicable
  type: boolean
- description: ''
  name: maxPenaltyAmount
  type: string
- description: ''
  name: descriptions
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-termandcondition-schema.json
slug: seatmap-display-termandcondition
source_filename: seatmap-display-termandcondition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TermAndCondition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"This defines what type of modification is concerned in this rule.\",\n      \"enum\": [\n        \"REFUND\",\n        \"EXCHANGE\",\n        \"REVALIDATION\",\n        \"REISSUE\",\n        \"REBOOK\",\n        \"CANCELLATION\"\n      ]\n    },\n    \"circumstances\": {\n      \"type\": \"string\"\n    },\n    \"notApplicable\": {\n      \"type\": \"boolean\"\n    },\n    \"maxPenaltyAmount\": {\n      \"type\": \"string\"\n    },\n    \"descriptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"properties\": {\n          \"descriptionType\": {\n            \"type\": \"string\"\n          },\n          \"text\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-termandcondition-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: TermAndCondition
---

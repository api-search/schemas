---
description: information about corporation
layout: schema
name: Corporation
properties_list:
- description: ''
  name: address
  type: object
- description: corporate information map. Possible keys key | name | - AU | Accounting Unit ON | Order Number DC | Department Code CC | Company Code CN | Company Name IA | Internal Account CE | Cost Centre EN | Empl
  name: info
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-corporation-schema.json
slug: transfer-booking-corporation
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Corporation\",\n  \"description\": \"information about corporation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"$ref\": \"#/definitions/AddressCommon\"\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"corporate information map. Possible keys\\n\\nkey    | name\\n | -\\nAU\\t   | Accounting Unit\\nON\\t   | Order Number\\nDC\\t   | Department Code\\nCC\\t   | Company Code\\nCN\\t   | Company Name\\nIA\\t   | Internal Account\\nCE\\t   | Cost Centre\\nEN\\t   | Employee Number\\nPN\\t   | Project Number\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-corporation-schema.json
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
title: Corporation
---

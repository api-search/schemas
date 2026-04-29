---
description: Error
layout: schema
name: Error
properties_list:
- description: '[Integer] A machine-readable error code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of error'
  name: code
  type: integer
- description: '[String] An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized'
  name: title
  type: string
- description: '[String] An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field value'
  name: detail
  type: string
- description: '[Integer] The [HTTP status code](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml) of this response. This is present only in terminal errors which cause an unsuccessful respo'
  name: status
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-error-schema.json
slug: hotel-booking-error
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Error\",\n  \"description\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"[Integer] A machine-readable error code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of error\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"[String] An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"[String] An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field value can be localized.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"[Integer]\
  \ The [HTTP status code](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml) of this response. This is present only in terminal errors which cause an unsuccessful response. In the case of multiple errors, they must all have the same status.\"\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"title\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-booking-error-schema.json
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
title: Error
---

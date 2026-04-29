---
description: A set of errors
layout: schema
name: Errors
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-errors-schema.json
slug: hotel-booking-errors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-errors-schema.json\",\n  \"title\": \"Errors\",\n  \"description\": \"A set of errors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"The Error Definition\",\n        \"title\": \"Error\",\n        \"properties\": {\n          \"status\": {\n            \"type\": \"integer\",\n            \"description\": \"The [HTTP status code](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml) of this response. This is present only in terminal errors which cause an unsuccessful response. In the case of multiple errors, they must all have the same status.\"\n          },\n          \"code\": {\n            \"type\": \"integer\",\n            \"description\"\
  : \"A machine-readable error code, that will enable the API Consumers code to handle this type of error\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized\"\n          },\n          \"detail\": {\n            \"type\": \"string\",\n            \"description\": \"An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field\\u2019s value can be localized.\"\n          },\n          \"source\": {\n            \"type\": \"object\",\n            \"title\": \"Error_Source\",\n            \"properties\": {\n              \"parameter\": {\n                \"type\": \"string\",\n                \"description\": \"The key of the URI path or query parameter that caused the error\"\n              },\n       \
  \       \"pointer\": {\n                \"type\": \"string\",\n                \"description\": \"A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error\"\n              },\n              \"example\": {\n                \"type\": \"string\",\n                \"description\": \"A sample input to guide the user when resolving this issue\"\n              }\n            }\n          },\n          \"documentation\": {\n            \"type\": \"string\",\n            \"format\": \"url\",\n            \"description\": \"A link to a web page or file with further documentation to help the API consumer resolve this error\"\n          }\n        },\n        \"example\": {\n          \"errors\": [\n            {\n              \"status\": 400,\n              \"code\": 477,\n              \"title\": \"INVALID FORMAT\",\n              \"detail\": \"invalid query parameter format\",\n              \"source\": {\n                \"parameter\": \"email\"\n         \
  \     }\n            }\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-errors-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Errors
---

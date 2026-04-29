---
description: ''
layout: schema
name: warnings
properties_list:
- description: A machine-readable error code from the Canned Messages table, that will enable the API Consumers code to handle this type of error
  name: code
  type: integer
- description: An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized
  name: title
  type: string
- description: An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field’s value can be
  name: detail
  type: string
- description: The Warning Source Definition
  name: source
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-routes-warnings-schema.json
slug: airline-routes-warnings
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"warnings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"A machine-readable error code from the Canned Messages table, that will enable the API Consumers code to handle this type of error\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field\\u2019s value can be localized.\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The Warning Source Definition\",\n      \"properties\": {\n     \
  \   \"parameter\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the URI path or query parameter that caused the error\"\n        },\n        \"pointer\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON Pointer RFC6901 to the associated entity in the request body that caused this error\"\n        },\n        \"example\": {\n          \"type\": \"string\",\n          \"description\": \"A sample input to guide the user when resolving this issue\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-routes-warnings-schema.json
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
title: warnings
---

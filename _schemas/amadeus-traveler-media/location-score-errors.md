---
description: errors schema
layout: schema
name: errors
properties_list:
- description: The [HTTP status code](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml) of this response. This is present only in terminal errors which cause an unsuccessful response. In th
  name: status
  type: integer
- description: A machine-readable error code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of error
  name: code
  type: integer
- description: An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized
  name: title
  type: string
- description: An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field’s value can be
  name: detail
  type: string
- description: ''
  name: source
  type: object
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/location-score-errors-schema.json
slug: location-score-errors
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/location-score-errors-schema.json\",\n  \"title\": \"errors\",\n  \"description\": \"errors schema\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"The [HTTP status code](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml) of this response. This is present only in terminal errors which cause an unsuccessful response. In the case of multiple errors, they must all have the same status.\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"A machine-readable error code from the Amadeus Canned Messages table, that will enable the API Consumers code to handle this type of error\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"An error title from the Canned Messages\
  \ table with a 1:1 correspondence to the error code. This may be localized\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the title, this field\\u2019s value can be localized.\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"title\": \"Error_Source\",\n      \"properties\": {\n        \"parameter\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the URI path or query parameter that caused the error\"\n        },\n        \"pointer\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error\"\n        },\n        \"example\": {\n          \"type\": \"string\",\n          \"description\": \"A sample input to guide the user when resolving this issue\"\
  \n        }\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/location-score-errors-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: errors
---

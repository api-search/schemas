---
description: The Warning Definition
layout: schema
name: Warning
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
- description: A link to a web page or file with further documentation to help the API consumer resolve this error
  name: documentation
  type: string
- description: ''
  name: sources
  type: array
- description: Indicate relationships from one entity to many other entities of any kind (e.g. from one passenger to their flight segments).
  name: relationships
  type: object
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-warning-schema.json
slug: hotel-booking-warning
source_filename: hotel-booking-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-warning-schema.json\",\n  \"title\": \"Warning\",\n  \"description\": \"The Warning Definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"A machine-readable error code from the Canned Messages table, that will enable the API Consumers code to handle this type of error\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"An error title from the Canned Messages table with a 1:1 correspondence to the error code. This may be localized\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"An easy-to-read explanation specific to this occurrence of the problem. It should give the API consumer an idea of what went wrong and how to recover from it. Like the\
  \ title, this field\\u2019s value can be localized.\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The Warning Source Definition\",\n      \"title\": \"Warning_Source\",\n      \"properties\": {\n        \"parameter\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the URI path or query parameter that caused the error\"\n        },\n        \"pointer\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON Pointer [RFC6901] to the associated entity in the request body that caused this error\"\n        },\n        \"example\": {\n          \"type\": \"string\",\n          \"description\": \"A sample input to guide the user when resolving this issue\"\n        }\n      }\n    },\n    \"documentation\": {\n      \"type\": \"string\",\n      \"format\": \"url\",\n      \"description\": \"A link to a web page or file with further documentation to help the API consumer resolve this error\"\n    },\n    \"sources\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Warning/properties/source\"\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Indicate relationships from one entity to many other entities of any kind (e.g. from one passenger to their flight segments).\",\n      \"title\": \"Relationships\",\n      \"properties\": {\n        \"collection\": {\n          \"type\": \"array\",\n          \"description\": \"The details of the related items\",\n          \"items\": {\n            \"description\": \"Relationship allows to cross reference 2 entities via Link and/or id .\",\n            \"title\": \"Relationship\",\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"id of the related resource\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"\
  description\": \"Type of the related resource\",\n                \"example\": \"processed-dcs-passenger\"\n              },\n              \"ref\": {\n                \"type\": \"string\",\n                \"format\": \"uri-reference\",\n                \"description\": \"Local reference of the related resource\"\n              },\n              \"targetSchema\": {\n                \"type\": \"string\",\n                \"description\": \"The targetSchema would be an instance of definition to be used for building the associated API Request operation\"\n              },\n              \"targetMediaType\": {\n                \"type\": \"string\",\n                \"description\": \"Related to \\\"targetSchema\\\", to be specified in case the media type is different for the referenced API request\"\n              },\n              \"hrefSchema\": {\n                \"type\": \"string\",\n                \"description\": \"type ( format, type, patterns, enum) definition for each URI parameters.\"\
  \n              },\n              \"href\": {\n                \"type\": \"string\",\n                \"format\": \"url\",\n                \"description\": \"URL value\"\n              },\n              \"methods\": {\n                \"type\": \"array\",\n                \"description\": \"HTTP methods supported by the sibling URI\",\n                \"items\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"GET\",\n                    \"POST\",\n                    \"PUT\",\n                    \"PATCH\",\n                    \"DELETE\",\n                    \"OPTIONS\"\n                  ]\n                }\n              },\n              \"rel\": {\n                \"type\": \"string\",\n                \"description\": \"Expose the type of relation between the current entity and the describe entity : https://www.iana.org/assignments/link-relations/link-relations.xhtml\"\n              }\n            }\n          }\n        }\n  \
  \    }\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-warning-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Warning
---

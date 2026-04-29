---
description: A request to purchase a offering.
layout: schema
name: PurchaseOfferingRequest
properties_list:
- description: ''
  name: ReservationName
  type: object
- description: ''
  name: Start
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-purchase-offering-request-schema.json
slug: mediaconnect-api-purchase-offering-request
source_filename: mediaconnect-api-purchase-offering-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-purchase-offering-request-schema.json\",\n  \"title\": \"PurchaseOfferingRequest\",\n  \"description\": \"A request to purchase a offering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservationName\"\n          },\n          \"description\": \"The name that you want to use for the reservation.\"\n        }\n      ]\n    },\n    \"Start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"start\"\n          },\n          \"description\": \"The date and time that you want the reservation to\
  \ begin, in Coordinated Universal Time (UTC). You can specify any date and time between 12:00am on the first day of the current month to the current time on today's date, inclusive. Specify the start in a 24-hour notation. Use the following format: YYYY-MM-DDTHH:mm:SSZ, where T and Z are literal characters. For example, to specify 11:30pm on March 5, 2020, enter 2020-03-05T23:30:00Z.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Start\",\n    \"ReservationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-purchase-offering-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: PurchaseOfferingRequest
---

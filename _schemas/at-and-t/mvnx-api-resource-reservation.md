---
description: ResourceReservation schema from AT&T API
layout: schema
name: ResourceReservation
properties_list:
- description: Unique reservation identifier
  name: id
  type: string
- description: ''
  name: href
  type: string
- description: Reservation state
  name: reservationState
  type: string
- description: ''
  name: reservedResource
  type: array
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-resource-reservation-schema.json
slug: mvnx-api-resource-reservation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-reservation-schema.json\",\n  \"title\": \"ResourceReservation\",\n  \"description\": \"ResourceReservation schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique reservation identifier\",\n      \"example\": \"reservation-500123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://devex-web.att.com/resourceReservation/reservation-500123\"\n    },\n    \"reservationState\": {\n      \"type\": \"string\",\n      \"description\": \"Reservation state\",\n      \"enum\": [\n        \"completed\",\n        \"cancelled\",\n        \"inProgress\"\n      ],\n      \"example\": \"completed\"\n    },\n    \"reservedResource\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Reserved phone number\",\n            \"example\": \"+12125559999\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-reservation-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: ResourceReservation
---

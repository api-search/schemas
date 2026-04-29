---
description: describes the relation between the current reservation and another one
layout: schema
name: AssociatedRecordCommon
properties_list:
- description: Record locator [Amadeus or OA] with which the current reservation is related. In case of a codeshare relation, it enables to identify the operating PNR.
  name: reference
  type: string
- description: Creation date of the referenced reservation. Date and time in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm:ss.sss format, e.g. 2019-07-09T12:30:00.000
  name: creationDate
  type: string
- description: Designates the system which has originated the referenced reservation.
  name: originSystemCode
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-associated-record-common-schema.json
slug: flight-create-orders-associated-record-common
source_filename: flight-create-orders-associated-record-common-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-associated-record-common-schema.json\",\n  \"title\": \"AssociatedRecordCommon\",\n  \"description\": \"describes the relation between the current reservation and another one\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Record locator [Amadeus or OA] with which the current reservation is related. In case of a codeshare relation, it enables to identify the operating PNR.\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Creation date of the referenced reservation. Date and time in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-ddThh:mm:ss.sss format, e.g. 2019-07-09T12:30:00.000\",\n      \"example\": \"2019-07-09T12:30:00.000\"\n    },\n    \"originSystemCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Designates the system which has originated the referenced reservation.\",\n      \"minLength\": 2,\n      \"maxLength\": 3\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-associated-record-common-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AssociatedRecordCommon
---

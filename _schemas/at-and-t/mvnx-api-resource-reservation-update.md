---
description: ResourceReservationUpdate schema from AT&T API
layout: schema
name: ResourceReservationUpdate
properties_list:
- description: Updated reservation state
  name: reservationState
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-resource-reservation-update-schema.json
slug: mvnx-api-resource-reservation-update
source_filename: mvnx-api-resource-reservation-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-reservation-update-schema.json\",\n  \"title\": \"ResourceReservationUpdate\",\n  \"description\": \"ResourceReservationUpdate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reservationState\": {\n      \"type\": \"string\",\n      \"description\": \"Updated reservation state\",\n      \"enum\": [\n        \"cancelled\"\n      ],\n      \"example\": \"cancelled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-reservation-update-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: ResourceReservationUpdate
---

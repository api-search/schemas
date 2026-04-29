---
description: ''
layout: schema
name: BookingGuest
properties_list:
- description: The unique identifier of the guest.
  name: id
  type: string
- description: The first name of the guest.
  name: first_name
  type: string
- description: The last name of the guest.
  name: last_name
  type: string
- description: The phone number of the guest.
  name: phone
  type: string
- description: Whether the guest has completed identity verification.
  name: verified
  type: boolean
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-booking-guest-schema.json
slug: airbnb-booking-guest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-booking-guest-schema.json\",\n  \"title\": \"BookingGuest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the guest.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the guest.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the guest.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the guest.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the guest has completed identity verification.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-booking-guest-schema.json
tags: []
title: BookingGuest
---

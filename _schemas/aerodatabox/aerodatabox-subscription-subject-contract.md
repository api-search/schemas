---
description: Describes subscription subject
layout: schema
name: SubscriptionSubjectContract
properties_list:
- description: ''
  name: type
  type: object
- description: Subject ID of a subscription. Complements SubjectType. E.g. SubjectType = "FlightNumber" and SubjectId = "DL 47" means that this subscription is for all updates of flight with number DL47.
  name: id
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-subscription-subject-contract-schema.json
slug: aerodatabox-subscription-subject-contract
source_filename: aerodatabox-subscription-subject-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscription-subject-contract-schema.json\",\n  \"title\": \"SubscriptionSubjectContract\",\n  \"description\": \"Describes subscription subject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/SubscriptionSubjectType\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Subject ID of a subscription. Complements SubjectType.\\r\\n\\r\\nE.g. SubjectType = \\\"FlightNumber\\\" and SubjectId = \\\"DL 47\\\" means that this\\r\\nsubscription is for all updates of flight with number DL47.\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscription-subject-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: SubscriptionSubjectContract
---

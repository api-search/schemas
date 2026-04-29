---
description: An equipment reservation at a core facility.
layout: schema
name: Reservation
properties_list:
- description: Unique identifier for the reservation.
  name: id
  type: integer
- description: Name of the reserved equipment.
  name: equipment_name
  type: string
- description: Reservation start time (ISO 8601).
  name: start_time
  type: string
- description: Reservation end time (ISO 8601).
  name: end_time
  type: string
- description: Username of the person who made the reservation.
  name: user
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-reservation-schema.json
slug: ilab-operations-api-reservation
source_filename: ilab-operations-api-reservation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-reservation-schema.json\",\n  \"title\": \"Reservation\",\n  \"description\": \"An equipment reservation at a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the reservation.\",\n      \"example\": 200456\n    },\n    \"equipment_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the reserved equipment.\",\n      \"example\": \"Illumina NovaSeq 6000\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Reservation start time (ISO 8601).\",\n      \"example\": \"2026-04-20T09:00:00Z\"\n    },\n    \"end_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"Reservation end time (ISO 8601).\",\n      \"example\": \"2026-04-20T17:00:00Z\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the person who made the reservation.\",\n      \"example\": \"jsmith\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-reservation-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Reservation
---

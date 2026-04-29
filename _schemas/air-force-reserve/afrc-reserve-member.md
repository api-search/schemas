---
description: An Air Force Reserve member record
layout: schema
name: ReserveMember
properties_list:
- description: Military service number or SSAN
  name: service_number
  type: string
- description: Military rank
  name: rank
  type: string
- description: Member last name
  name: last_name
  type: string
- description: Member first name
  name: first_name
  type: string
- description: Assigned reserve unit
  name: unit
  type: string
- description: Air Force Specialty Code (career field)
  name: afsc
  type: string
- description: Current duty status
  name: duty_status
  type: string
- description: Date of enlistment
  name: enlistment_date
  type: string
provider_name: Air Force Reserve
provider_slug: air-force-reserve
schema_file: json-schema/afrc-reserve-member-schema.json
slug: afrc-reserve-member
source_filename: afrc-reserve-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/json-schema/afrc-reserve-member-schema.json\",\n  \"title\": \"ReserveMember\",\n  \"description\": \"An Air Force Reserve member record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_number\": {\n      \"type\": \"string\",\n      \"description\": \"Military service number or SSAN\",\n      \"example\": \"123-45-6789\"\n    },\n    \"rank\": {\n      \"type\": \"string\",\n      \"description\": \"Military rank\",\n      \"example\": \"Technical Sergeant\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Member last name\",\n      \"example\": \"Smith\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Member first name\",\n      \"example\": \"John\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Assigned reserve unit\",\n      \"example\": \"433rd Airlift Wing\"\n    },\n    \"afsc\": {\n      \"type\": \"string\",\n      \"description\": \"Air Force Specialty Code (career field)\",\n      \"example\": \"1A2X1\"\n    },\n    \"duty_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current duty status\",\n      \"example\": \"Traditional Reservist\"\n    },\n    \"enlistment_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of enlistment\",\n      \"example\": \"2020-06-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/json-schema/afrc-reserve-member-schema.json
tags:
- Federal Government
- Military
- Defense
- Air Force
- United States Government
title: ReserveMember
---

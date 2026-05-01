---
description: DescribeReservationResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DescribeReservationResponse
properties_list:
- description: ''
  name: Reservation
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-describe-reservation-response-schema.json
slug: mediaconnect-api-describe-reservation-response
source_filename: mediaconnect-api-describe-reservation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-reservation-response-schema.json\",\n  \"title\": \"DescribeReservationResponse\",\n  \"description\": \"DescribeReservationResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Reservation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reservation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservation\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-reservation-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: DescribeReservationResponse
---

---
description: Request to update a reservation
layout: schema
name: UpdateReservationRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RenewalSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-reservation-request-schema.json
slug: medialive-api-update-reservation-request
source_filename: medialive-api-update-reservation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-reservation-request-schema.json\",\n  \"title\": \"UpdateReservationRequest\",\n  \"description\": \"Request to update a reservation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of the reservation\"\n        }\n      ]\n    },\n    \"RenewalSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenewalSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renewalSettings\"\n          },\n          \"description\": \"Renewal settings for the reservation\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-reservation-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateReservationRequest
---

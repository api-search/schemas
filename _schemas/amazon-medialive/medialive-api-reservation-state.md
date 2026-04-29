---
description: Current reservation state
layout: schema
name: ReservationState
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-reservation-state-schema.json
slug: medialive-api-reservation-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reservation-state-schema.json\",\n  \"title\": \"ReservationState\",\n  \"description\": \"Current reservation state\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACTIVE\",\n    \"EXPIRED\",\n    \"CANCELED\",\n    \"DELETED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reservation-state-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ReservationState
---

---
description: Resolution based on lines of vertical resolution; SD is less than 720 lines, HD is 720 to 1080 lines, FHD is 1080 lines, UHD is greater than 1080 lines
layout: schema
name: ReservationResolution
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-reservation-resolution-schema.json
slug: medialive-api-reservation-resolution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reservation-resolution-schema.json\",\n  \"title\": \"ReservationResolution\",\n  \"description\": \"Resolution based on lines of vertical resolution; SD is less than 720 lines, HD is 720 to 1080 lines, FHD is 1080 lines, UHD is greater than 1080 lines\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SD\",\n    \"HD\",\n    \"FHD\",\n    \"UHD\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reservation-resolution-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ReservationResolution
---

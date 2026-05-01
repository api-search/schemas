---
description: Corresponds to the device_restrictions parameter in a segmentation_descriptor. If you include one of the "restriction" flags then you must include all four of them.
layout: schema
name: Scte35DeviceRestrictions
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-device-restrictions-schema.json
slug: medialive-api-scte35-device-restrictions
source_filename: medialive-api-scte35-device-restrictions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-device-restrictions-schema.json\",\n  \"title\": \"Scte35DeviceRestrictions\",\n  \"description\": \"Corresponds to the device_restrictions parameter in a segmentation_descriptor. If you include one of the \\\"restriction\\\" flags then you must include all four of them.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"RESTRICT_GROUP0\",\n    \"RESTRICT_GROUP1\",\n    \"RESTRICT_GROUP2\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-device-restrictions-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35DeviceRestrictions
---

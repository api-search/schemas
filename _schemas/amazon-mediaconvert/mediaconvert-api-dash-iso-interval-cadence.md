---
description: The cadence MediaConvert follows for generating thumbnails. If set to FOLLOW_IFRAME, MediaConvert generates thumbnails for each IDR frame in the output (matching the GOP cadence). If set to FOLLOW_CUSTOM, MediaConvert generates thumbnails according to the interval you specify in thumbnailInterval.
layout: schema
name: DashIsoIntervalCadence
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-iso-interval-cadence-schema.json
slug: mediaconvert-api-dash-iso-interval-cadence
source_filename: mediaconvert-api-dash-iso-interval-cadence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-interval-cadence-schema.json\",\n  \"title\": \"DashIsoIntervalCadence\",\n  \"description\": \"The cadence MediaConvert follows for generating thumbnails. If set to FOLLOW_IFRAME, MediaConvert generates thumbnails for each IDR frame in the output (matching the GOP cadence). If set to FOLLOW_CUSTOM, MediaConvert generates thumbnails according to the interval you specify in thumbnailInterval.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FOLLOW_IFRAME\",\n    \"FOLLOW_CUSTOM\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-interval-cadence-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DashIsoIntervalCadence
---

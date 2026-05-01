---
description: Specify how often MediaConvert sends STATUS_UPDATE events to Amazon CloudWatch Events. Set the interval, in seconds, between status updates. MediaConvert sends an update at this interval from the time the service begins processing your job to the time it completes the transcode or encounters an error.
layout: schema
name: StatusUpdateInterval
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-status-update-interval-schema.json
slug: mediaconvert-api-status-update-interval
source_filename: mediaconvert-api-status-update-interval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-status-update-interval-schema.json\",\n  \"title\": \"StatusUpdateInterval\",\n  \"description\": \"Specify how often MediaConvert sends STATUS_UPDATE events to Amazon CloudWatch Events. Set the interval, in seconds, between status updates. MediaConvert sends an update at this interval from the time the service begins processing your job to the time it completes the transcode or encounters an error.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SECONDS_10\",\n    \"SECONDS_12\",\n    \"SECONDS_15\",\n    \"SECONDS_20\",\n    \"SECONDS_30\",\n    \"SECONDS_60\",\n    \"SECONDS_120\",\n    \"SECONDS_180\",\n    \"SECONDS_240\",\n    \"SECONDS_300\",\n    \"SECONDS_360\",\n    \"SECONDS_420\",\n    \"SECONDS_480\",\n    \"SECONDS_540\",\n    \"SECONDS_600\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-status-update-interval-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: StatusUpdateInterval
---

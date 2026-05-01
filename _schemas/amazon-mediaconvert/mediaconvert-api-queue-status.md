---
description: Queues can be ACTIVE or PAUSED. If you pause a queue, jobs in that queue won't begin. Jobs that are running when you pause a queue continue to run until they finish or result in an error.
layout: schema
name: QueueStatus
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-queue-status-schema.json
slug: mediaconvert-api-queue-status
source_filename: mediaconvert-api-queue-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-status-schema.json\",\n  \"title\": \"QueueStatus\",\n  \"description\": \"Queues can be ACTIVE or PAUSED. If you pause a queue, jobs in that queue won't begin. Jobs that are running when you pause a queue continue to run until they finish or result in an error.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACTIVE\",\n    \"PAUSED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-status-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: QueueStatus
---

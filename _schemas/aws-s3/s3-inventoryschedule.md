---
description: Specifies the schedule for generating inventory results.
layout: schema
name: InventorySchedule
properties_list:
- description: ''
  name: Frequency
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventoryschedule-schema.json
slug: s3-inventoryschedule
source_filename: s3-inventoryschedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventorySchedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Frequency\": {}\n  },\n  \"required\": [\n    \"Frequency\"\n  ],\n  \"description\": \"Specifies the schedule for generating inventory results.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inventoryschedule-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
title: InventorySchedule
---

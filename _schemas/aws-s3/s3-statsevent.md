---
description: Container for the Stats Event.
layout: schema
name: StatsEvent
properties_list:
- description: ''
  name: Details
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-statsevent-schema.json
slug: s3-statsevent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatsEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Details\": {}\n  },\n  \"description\": \"Container for the Stats Event.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-statsevent-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: StatsEvent
---

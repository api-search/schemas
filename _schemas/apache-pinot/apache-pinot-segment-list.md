---
description: SegmentList schema from Apache Pinot
layout: schema
name: SegmentList
properties_list:
- description: ''
  name: OFFLINE
  type: array
- description: ''
  name: REALTIME
  type: array
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-segment-list-schema.json
slug: apache-pinot-segment-list
source_filename: apache-pinot-segment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-segment-list-schema.json\",\n  \"title\": \"SegmentList\",\n  \"description\": \"SegmentList schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OFFLINE\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"REALTIME\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-segment-list-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: SegmentList
---

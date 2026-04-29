---
description: A single instant on the Hudi timeline representing a completed action
layout: schema
name: TimelineInstant
properties_list:
- description: Instant timestamp (yyyyMMddHHmmssSSS format)
  name: timestamp
  type: string
- description: Action type (commit, deltacommit, compaction, clean, rollback)
  name: action
  type: string
- description: Instant state (COMPLETED, INFLIGHT, REQUESTED)
  name: state
  type: string
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-timelineinstant-schema.json
slug: hudi-timelineinstant
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hudi/json-schema/hudi-timelineinstant-schema.json\",\n  \"title\": \"TimelineInstant\",\n  \"type\": \"object\",\n  \"description\": \"A single instant on the Hudi timeline representing a completed action\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Instant timestamp (yyyyMMddHHmmssSSS format)\",\n      \"example\": \"20240101120000000\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action type (commit, deltacommit, compaction, clean, rollback)\",\n      \"example\": \"commit\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Instant state (COMPLETED, INFLIGHT, REQUESTED)\",\n      \"example\": \"COMPLETED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hudi/refs/heads/main/json-schema/hudi-timelineinstant-schema.json
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: TimelineInstant
---

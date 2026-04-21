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

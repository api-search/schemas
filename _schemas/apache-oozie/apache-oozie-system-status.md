---
description: Oozie system mode status.
layout: schema
name: SystemStatus
properties_list:
- description: Current system mode.
  name: systemMode
  type: string
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-system-status-schema.json
slug: apache-oozie-system-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-system-status-schema.json\",\n  \"title\": \"SystemStatus\",\n  \"description\": \"Oozie system mode status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"systemMode\": {\n      \"type\": \"string\",\n      \"description\": \"Current system mode.\",\n      \"enum\": [\n        \"NORMAL\",\n        \"NOWEBSERVICE\",\n        \"SAFEMODE\"\n      ],\n      \"example\": \"NORMAL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-system-status-schema.json
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: SystemStatus
---

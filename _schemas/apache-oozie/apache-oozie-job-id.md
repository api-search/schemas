---
description: Job submission response containing the assigned job ID.
layout: schema
name: JobId
properties_list:
- description: The Oozie job identifier assigned to the submitted job.
  name: id
  type: string
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-job-id-schema.json
slug: apache-oozie-job-id
source_filename: apache-oozie-job-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-job-id-schema.json\",\n  \"title\": \"JobId\",\n  \"description\": \"Job submission response containing the assigned job ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Oozie job identifier assigned to the submitted job.\",\n      \"example\": \"0000001-200101120000000-oozie-admin-W\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-job-id-schema.json
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: JobId
---

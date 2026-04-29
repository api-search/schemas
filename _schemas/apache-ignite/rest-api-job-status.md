---
description: Job status.
layout: schema
name: JobStatus
properties_list: []
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-job-status-schema.json
slug: rest-api-job-status
source_filename: rest-api-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"description\": \"Job status.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"QUEUED\",\n    \"EXECUTING\",\n    \"FAILED\",\n    \"COMPLETED\",\n    \"CANCELING\",\n    \"CANCELED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-job-status-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: JobStatus
---

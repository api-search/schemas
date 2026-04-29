---
description: DTO of update job priority request body.
layout: schema
name: UpdateJobPriorityBody
properties_list:
- description: Priority.
  name: priority
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-update-job-priority-body-schema.json
slug: rest-api-update-job-priority-body
source_filename: rest-api-update-job-priority-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-update-job-priority-body-schema.json\",\n  \"title\": \"UpdateJobPriorityBody\",\n  \"description\": \"DTO of update job priority request body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority.\",\n      \"format\": \"int32\"\n    }\n  },\n  \"required\": [\n    \"priority\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-update-job-priority-body-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: UpdateJobPriorityBody
---

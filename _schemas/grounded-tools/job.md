---
description: An indexing pipeline job that tracks the progress and status of a documentation scraping operation.
layout: schema
name: grounded.tools Job
properties_list:
- description: Unique job identifier.
  name: id
  type: string
- description: Library name being indexed.
  name: library
  type: string
- description: Library version being indexed.
  name: version
  type: string
- description: Current job status.
  name: status
  type: string
- description: Timestamp when the job was created.
  name: createdAt
  type: string
- description: Timestamp when the job started processing.
  name: startedAt
  type: string
- description: Timestamp when the job completed.
  name: finishedAt
  type: string
- description: Error message if the job failed.
  name: error
  type: string
- description: Progress information for the job.
  name: progress
  type: object
provider_name: Grounded.tools
provider_slug: grounded-tools
schema_file: json-schema/job.json
slug: job
source_filename: job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/grounded-tools/blob/main/json-schema/job.json\",\n  \"title\": \"grounded.tools Job\",\n  \"description\": \"An indexing pipeline job that tracks the progress and status of a documentation scraping operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique job identifier.\"\n    },\n    \"library\": {\n      \"type\": \"string\",\n      \"description\": \"Library name being indexed.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Library version being indexed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"queued\",\n        \"running\",\n        \"completed\",\n        \"failed\",\n        \"cancelling\",\n        \"cancelled\"\n      ],\n      \"description\"\
  : \"Current job status.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was created.\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Timestamp when the job started processing.\"\n    },\n    \"finishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Timestamp when the job completed.\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Error message if the job failed.\"\n    },\n    \"progress\": {\n      \"type\": \"object\",\n      \"description\": \"Progress information for the job.\",\n      \"properties\": {\n        \"pages\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of pages processed so far.\"\n        },\n        \"totalPages\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Total pages to process.\"\n        },\n        \"totalDiscovered\": {\n          \"type\": \"integer\",\n          \"description\": \"Total pages discovered during crawling.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"library\",\n    \"status\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grounded-tools/refs/heads/main/json-schema/job.json
tags:
- Developer Tools
- Developers
- Documentation
- Experience
title: grounded.tools Job
---

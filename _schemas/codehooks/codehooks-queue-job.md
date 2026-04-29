---
description: A job in the Codehooks asynchronous queue system. Jobs are enqueued to named topics and processed by registered worker functions.
layout: schema
name: Codehooks Queue Job
properties_list:
- description: Unique identifier of the enqueued job.
  name: _id
  type: string
- description: The queue topic name the job belongs to.
  name: topic
  type: string
- description: The job payload data to be processed by the worker function.
  name: payload
  type: object
- description: The current processing status of the job.
  name: status
  type: string
- description: Timestamp when the job was enqueued.
  name: createdAt
  type: string
- description: Timestamp when the job finished processing.
  name: completedAt
  type: string
provider_name: Codehooks
provider_slug: codehooks
schema_file: json-schema/codehooks-queue-job-schema.json
slug: codehooks-queue-job
source_filename: codehooks-queue-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/json-schema/codehooks-queue-job-schema.json\",\n  \"title\": \"Codehooks Queue Job\",\n  \"description\": \"A job in the Codehooks asynchronous queue system. Jobs are enqueued to named topics and processed by registered worker functions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the enqueued job.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"The queue topic name the job belongs to.\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The job payload data to be processed by the worker function.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"processing\", \"completed\", \"failed\"\
  ],\n      \"description\": \"The current processing status of the job.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job was enqueued.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job finished processing.\"\n    }\n  },\n  \"required\": [\"_id\", \"topic\", \"payload\"],\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"_id\": \"job-64a1b2c3d4e5f600\",\n      \"topic\": \"send-email\",\n      \"payload\": {\n        \"to\": \"user@example.com\",\n        \"subject\": \"Welcome\",\n        \"body\": \"Hello and welcome!\"\n      },\n      \"status\": \"pending\",\n      \"createdAt\": \"2025-06-01T12:00:00.000Z\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/json-schema/codehooks-queue-job-schema.json
tags:
- Backend
- Database
- Events
- Hooks
- JavaScript
- NoSQL
- Queues
- Serverless
- Webhooks
- Workers
- Workflows
title: Codehooks Queue Job
---

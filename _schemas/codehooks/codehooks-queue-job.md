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

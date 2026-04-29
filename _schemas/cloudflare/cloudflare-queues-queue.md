---
description: ''
layout: schema
name: Queue
properties_list:
- description: The unique identifier of the queue.
  name: queue_id
  type: string
- description: The name of the queue.
  name: queue_name
  type: string
- description: When the queue was created.
  name: created_on
  type: string
- description: When the queue was last modified.
  name: modified_on
  type: string
- description: Number of producers attached.
  name: producers_total_count
  type: integer
- description: Number of consumers attached.
  name: consumers_total_count
  type: integer
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-queues-queue-schema.json
slug: cloudflare-queues-queue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Queue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queue_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the queue.\"\n    },\n    \"queue_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the queue.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"When the queue was created.\"\n    },\n    \"modified_on\": {\n      \"type\": \"string\",\n      \"description\": \"When the queue was last modified.\"\n    },\n    \"producers_total_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of producers attached.\"\n    },\n    \"consumers_total_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consumers attached.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-queues-queue-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: Queue
---

---
description: High-level cluster overview
layout: schema
name: ClusterOverview
properties_list:
- description: Number of worker nodes
  name: workers
  type: integer
- description: Number of running jobs
  name: runningJobs
  type: integer
- description: Number of finished jobs
  name: finishedJobs
  type: integer
- description: Number of failed jobs
  name: failedJobs
  type: integer
- description: Number of canceled jobs
  name: canceledJobs
  type: integer
- description: Total available task slots
  name: totalSlot
  type: integer
- description: Currently used task slots
  name: usedSlot
  type: integer
provider_name: Apache SeaTunnel
provider_slug: apache-seatunnel
schema_file: json-schema/apache-seatunnel-cluster-overview-schema.json
slug: apache-seatunnel-cluster-overview
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-cluster-overview-schema.json\",\n  \"title\": \"ClusterOverview\",\n  \"description\": \"High-level cluster overview\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of worker nodes\"\n    },\n    \"runningJobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of running jobs\"\n    },\n    \"finishedJobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of finished jobs\"\n    },\n    \"failedJobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of failed jobs\"\n    },\n    \"canceledJobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of canceled jobs\"\n    },\n    \"totalSlot\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Total available task slots\"\n    },\n    \"usedSlot\": {\n      \"type\": \"integer\",\n      \"description\": \"Currently used task slots\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-seatunnel/refs/heads/main/json-schema/apache-seatunnel-cluster-overview-schema.json
tags:
- Data Integration
- ETL
- ELT
- Batch
- Streaming
- Apache
- Open Source
title: ClusterOverview
---

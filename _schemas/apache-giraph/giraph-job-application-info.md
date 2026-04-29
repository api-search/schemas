---
description: YARN application (Giraph job) status information
layout: schema
name: ApplicationInfo
properties_list:
- description: YARN application ID
  name: id
  type: string
- description: Application name (usually Giraph followed by the algorithm name)
  name: name
  type: string
- description: Application type (MAPREDUCE for Giraph)
  name: applicationType
  type: string
- description: Current application state
  name: state
  type: string
- description: Final status after completion
  name: finalStatus
  type: string
- description: Job completion percentage (0-100)
  name: progress
  type: number
- description: URL for job tracking UI
  name: trackingUrl
  type: string
- description: YARN queue name
  name: queue
  type: string
- description: Job start time in milliseconds since epoch
  name: startedTime
  type: integer
- description: Job finish time in milliseconds (0 if still running)
  name: finishedTime
  type: integer
- description: Elapsed time in milliseconds
  name: elapsedTime
  type: integer
- description: Number of running containers
  name: numContainers
  type: integer
provider_name: Apache Giraph
provider_slug: apache-giraph
schema_file: json-schema/giraph-job-application-info-schema.json
slug: giraph-job-application-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-application-info-schema.json\",\n  \"title\": \"ApplicationInfo\",\n  \"description\": \"YARN application (Giraph job) status information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"YARN application ID\",\n      \"example\": \"application_1718153645993_0001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name (usually Giraph followed by the algorithm name)\",\n      \"example\": \"Giraph PageRank\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\",\n      \"description\": \"Application type (MAPREDUCE for Giraph)\",\n      \"example\": \"MAPREDUCE\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current application state\",\n \
  \     \"enum\": [\n        \"NEW\",\n        \"NEW_SAVING\",\n        \"SUBMITTED\",\n        \"ACCEPTED\",\n        \"RUNNING\",\n        \"FINISHED\",\n        \"FAILED\",\n        \"KILLED\"\n      ],\n      \"example\": \"RUNNING\"\n    },\n    \"finalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Final status after completion\",\n      \"enum\": [\n        \"UNDEFINED\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"KILLED\"\n      ],\n      \"example\": \"UNDEFINED\"\n    },\n    \"progress\": {\n      \"type\": \"number\",\n      \"description\": \"Job completion percentage (0-100)\",\n      \"example\": \"50.0\"\n    },\n    \"trackingUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL for job tracking UI\",\n      \"example\": \"http://localhost:8088/proxy/application_1718153645993_0001/\"\n    },\n    \"queue\": {\n      \"type\": \"string\",\n      \"description\": \"YARN queue name\",\n      \"example\": \"default\"\n    },\n  \
  \  \"startedTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Job start time in milliseconds since epoch\",\n      \"example\": \"1718153645993\"\n    },\n    \"finishedTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Job finish time in milliseconds (0 if still running)\",\n      \"example\": \"0\"\n    },\n    \"elapsedTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Elapsed time in milliseconds\",\n      \"example\": \"30000\"\n    },\n    \"numContainers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of running containers\",\n      \"example\": \"4\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/json-schema/giraph-job-application-info-schema.json
tags:
- Apache
- Big Data
- BSP
- Graph Processing
- Hadoop
- Open Source
- Retired
title: ApplicationInfo
---

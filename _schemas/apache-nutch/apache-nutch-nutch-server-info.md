---
description: Status information about the running Nutch server.
layout: schema
name: NutchServerInfo
properties_list:
- description: The date and time the server was started.
  name: startDate
  type: string
- description: Set of known configuration IDs.
  name: configuration
  type: array
- description: All jobs (any state).
  name: jobs
  type: array
- description: Currently running jobs.
  name: runningJobs
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-nutch-server-info-schema.json
slug: apache-nutch-nutch-server-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-nutch-server-info-schema.json\",\n  \"title\": \"NutchServerInfo\",\n  \"description\": \"Status information about the running Nutch server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the server was started.\"\n    },\n    \"configuration\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"uniqueItems\": true,\n      \"description\": \"Set of known configuration IDs.\"\n    },\n    \"jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Information about a crawl job.\",\n        \"required\": [\n          \"type\",\n          \"state\"\n        ],\n\
  \        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique job identifier.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of Nutch crawl job.\",\n            \"enum\": [\n              \"INJECT\",\n              \"GENERATE\",\n              \"FETCH\",\n              \"PARSE\",\n              \"UPDATEDB\",\n              \"INDEX\",\n              \"READDB\",\n              \"CLASS\",\n              \"INVERTLINKS\",\n              \"DEDUP\"\n            ]\n          },\n          \"confId\": {\n            \"type\": \"string\",\n            \"description\": \"The configuration ID used for this job.\"\n          },\n          \"args\": {\n            \"type\": \"object\",\n            \"additionalProperties\": true,\n            \"description\": \"Arguments passed to the job.\"\n          },\n          \"result\": {\n            \"type\": \"object\",\n   \
  \         \"additionalProperties\": true,\n            \"description\": \"Result data returned after job completion.\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current state of a job.\",\n            \"enum\": [\n              \"IDLE\",\n              \"RUNNING\",\n              \"FINISHED\",\n              \"FAILED\",\n              \"KILLED\",\n              \"STOPPING\",\n              \"KILLING\",\n              \"ANY\"\n            ]\n          },\n          \"msg\": {\n            \"type\": \"string\",\n            \"description\": \"A human-readable status or error message.\"\n          },\n          \"crawlId\": {\n            \"type\": \"string\",\n            \"description\": \"The crawl identifier associated with this job.\"\n          }\n        }\n      },\n      \"description\": \"All jobs (any state).\"\n    },\n    \"runningJobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"\
  object\",\n        \"description\": \"Information about a crawl job.\",\n        \"required\": [\n          \"type\",\n          \"state\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique job identifier.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of Nutch crawl job.\",\n            \"enum\": [\n              \"INJECT\",\n              \"GENERATE\",\n              \"FETCH\",\n              \"PARSE\",\n              \"UPDATEDB\",\n              \"INDEX\",\n              \"READDB\",\n              \"CLASS\",\n              \"INVERTLINKS\",\n              \"DEDUP\"\n            ]\n          },\n          \"confId\": {\n            \"type\": \"string\",\n            \"description\": \"The configuration ID used for this job.\"\n          },\n          \"args\": {\n            \"type\": \"object\",\n            \"additionalProperties\"\
  : true,\n            \"description\": \"Arguments passed to the job.\"\n          },\n          \"result\": {\n            \"type\": \"object\",\n            \"additionalProperties\": true,\n            \"description\": \"Result data returned after job completion.\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current state of a job.\",\n            \"enum\": [\n              \"IDLE\",\n              \"RUNNING\",\n              \"FINISHED\",\n              \"FAILED\",\n              \"KILLED\",\n              \"STOPPING\",\n              \"KILLING\",\n              \"ANY\"\n            ]\n          },\n          \"msg\": {\n            \"type\": \"string\",\n            \"description\": \"A human-readable status or error message.\"\n          },\n          \"crawlId\": {\n            \"type\": \"string\",\n            \"description\": \"The crawl identifier associated with this job.\"\n          }\n        }\n      },\n  \
  \    \"description\": \"Currently running jobs.\"\n    }\n  },\n  \"required\": [\n    \"configuration\",\n    \"jobs\",\n    \"runningJobs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-nutch-server-info-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: NutchServerInfo
---

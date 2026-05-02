---
description: A Spark batch job submission resource for running big data processing workloads.
layout: schema
name: Azure Synapse Analytics Spark Batch Job
properties_list:
- description: The batch job ID.
  name: id
  type: integer
- description: The name of the batch job.
  name: name
  type: string
- description: ''
  name: workspaceName
  type: string
- description: ''
  name: sparkPoolName
  type: string
- description: ''
  name: submitterName
  type: string
- description: ''
  name: submitterId
  type: string
- description: ''
  name: artifactId
  type: string
- description: ''
  name: jobType
  type: string
- description: ''
  name: result
  type: string
- description: The batch state.
  name: state
  type: string
- description: The Spark application ID.
  name: appId
  type: string
- description: ''
  name: appInfo
  type: object
- description: Log lines for the batch job.
  name: log
  type: array
- description: ''
  name: livyInfo
  type: object
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-spark-batch-job-schema.json
slug: azure-synapse-analytics-spark-batch-job
source_filename: azure-synapse-analytics-spark-batch-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-spark-batch-job-schema.json\",\n  \"title\": \"Azure Synapse Analytics Spark Batch Job\",\n  \"description\": \"A Spark batch job submission resource for running big data processing workloads.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The batch job ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the batch job.\"\n    },\n    \"workspaceName\": {\n      \"type\": \"string\"\n    },\n    \"sparkPoolName\": {\n      \"type\": \"string\"\n    },\n    \"submitterName\": {\n      \"type\": \"string\"\n    },\n    \"submitterId\": {\n      \"type\": \"string\"\n    },\n    \"artifactId\": {\n      \"type\": \"string\"\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\"SparkBatch\", \"SparkSession\"]\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\"Uncertain\", \"Succeeded\", \"Failed\", \"Cancelled\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The batch state.\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The Spark application ID.\"\n    },\n    \"appInfo\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"log\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Log lines for the batch job.\"\n    },\n    \"livyInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"currentState\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-spark-batch-job-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Spark Batch Job
---

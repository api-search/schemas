---
description: ''
layout: schema
name: Job
properties_list:
- description: Canonical identifier of the job
  name: job_id
  type: integer
- description: Username of the job creator
  name: creator_user_name
  type: string
- description: User the job runs as
  name: run_as_user_name
  type: string
- description: Time the job was created (epoch milliseconds)
  name: created_time
  type: integer
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schema_file: json-schema/azure-databricks-job-schema.json
slug: azure-databricks-job
source_filename: azure-databricks-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Canonical identifier of the job\"\n    },\n    \"creator_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the job creator\"\n    },\n    \"run_as_user_name\": {\n      \"type\": \"string\",\n      \"description\": \"User the job runs as\"\n    },\n    \"created_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Time the job was created (epoch milliseconds)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-databricks/refs/heads/main/json-schema/azure-databricks-job-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: Job
---

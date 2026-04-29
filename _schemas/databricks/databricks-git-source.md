---
description: ''
layout: schema
name: GitSource
properties_list:
- description: URL of the Git repository.
  name: git_url
  type: string
- description: The Git provider.
  name: git_provider
  type: string
- description: Branch to use.
  name: git_branch
  type: string
- description: Tag to use.
  name: git_tag
  type: string
- description: Commit hash to use.
  name: git_commit
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-git-source-schema.json
slug: databricks-git-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GitSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"git_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the Git repository.\"\n    },\n    \"git_provider\": {\n      \"type\": \"string\",\n      \"description\": \"The Git provider.\"\n    },\n    \"git_branch\": {\n      \"type\": \"string\",\n      \"description\": \"Branch to use.\"\n    },\n    \"git_tag\": {\n      \"type\": \"string\",\n      \"description\": \"Tag to use.\"\n    },\n    \"git_commit\": {\n      \"type\": \"string\",\n      \"description\": \"Commit hash to use.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-git-source-schema.json
tags:
- AI
- Analytics
- Apache Spark
- Big Data
- Clean Rooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
title: GitSource
---

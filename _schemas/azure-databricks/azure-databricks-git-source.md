---
description: ''
layout: schema
name: GitSource
properties_list:
- description: URL of the Git repository
  name: git_url
  type: string
- description: Git provider type
  name: git_provider
  type: string
- description: Branch to check out
  name: git_branch
  type: string
- description: Tag to check out
  name: git_tag
  type: string
- description: Commit hash to check out
  name: git_commit
  type: string
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-git-source-schema.json
slug: azure-databricks-git-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GitSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"git_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the Git repository\"\n    },\n    \"git_provider\": {\n      \"type\": \"string\",\n      \"description\": \"Git provider type\"\n    },\n    \"git_branch\": {\n      \"type\": \"string\",\n      \"description\": \"Branch to check out\"\n    },\n    \"git_tag\": {\n      \"type\": \"string\",\n      \"description\": \"Tag to check out\"\n    },\n    \"git_commit\": {\n      \"type\": \"string\",\n      \"description\": \"Commit hash to check out\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-git-source-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: GitSource
---

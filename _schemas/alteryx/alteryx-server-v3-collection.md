---
description: A collection of workflows, schedules, and users
layout: schema
name: Collection
properties_list:
- description: Unique collection identifier
  name: id
  type: string
- description: Name of the collection
  name: name
  type: string
- description: ID of the collection owner
  name: ownerId
  type: string
- description: Date the collection was created
  name: dateCreated
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-collection-schema.json
slug: alteryx-server-v3-collection
source_filename: alteryx-server-v3-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Collection\",\n  \"type\": \"object\",\n  \"description\": \"A collection of workflows, schedules, and users\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique collection identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the collection\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the collection owner\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Date the collection was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-collection-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: Collection
---

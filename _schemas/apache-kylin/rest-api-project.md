---
description: A Kylin project
layout: schema
name: Project
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Creation time as Unix timestamp
  name: createTimeUTC
  type: integer
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-project-schema.json
slug: rest-api-project
source_filename: rest-api-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"A Kylin project\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"learn_kylin\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Learning project for Apache Kylin\"\n    },\n    \"createTimeUTC\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation time as Unix timestamp\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-project-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: Project
---

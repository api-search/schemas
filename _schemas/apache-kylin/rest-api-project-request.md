---
description: Request to create a project
layout: schema
name: ProjectRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-project-request-schema.json
slug: rest-api-project-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-project-request-schema.json\",\n  \"title\": \"ProjectRequest\",\n  \"description\": \"Request to create a project\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my_project\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"My Kylin project\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-project-request-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: ProjectRequest
---

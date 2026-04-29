---
description: Current session state
layout: schema
name: SessionState
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: state
  type: string
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-session-state-schema.json
slug: rest-api-session-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-session-state-schema.json\",\n  \"title\": \"SessionState\",\n  \"description\": \"Current session state\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"idle\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-session-state-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: SessionState
---

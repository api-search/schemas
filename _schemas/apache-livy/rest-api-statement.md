---
description: A code statement executed in a session
layout: schema
name: Statement
properties_list:
- description: Statement identifier
  name: id
  type: integer
- description: The code that was executed
  name: code
  type: string
- description: Statement execution state
  name: state
  type: string
- description: Statement output
  name: output
  type: object
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-statement-schema.json
slug: rest-api-statement
source_filename: rest-api-statement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-statement-schema.json\",\n  \"title\": \"Statement\",\n  \"description\": \"A code statement executed in a session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Statement identifier\",\n      \"example\": 0\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The code that was executed\",\n      \"example\": \"sc.parallelize([1,2,3]).count()\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Statement execution state\",\n      \"enum\": [\n        \"waiting\",\n        \"running\",\n        \"available\",\n        \"error\",\n        \"cancelling\",\n        \"cancelled\"\n      ],\n      \"example\": \"available\"\n    },\n    \"output\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Statement output\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"example\": \"ok\"\n        },\n        \"execution_count\": {\n          \"type\": \"integer\",\n          \"example\": 0\n        },\n        \"data\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-statement-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Statement
---

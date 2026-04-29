---
description: ScriptRequest schema from Apache Pig
layout: schema
name: ScriptRequest
properties_list:
- description: ''
  name: script
  type: string
provider_name: Apache Pig
provider_slug: apache-pig
schema_file: json-schema/apache-pig-script-request-schema.json
slug: apache-pig-script-request
source_filename: apache-pig-script-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-script-request-schema.json\",\n  \"title\": \"ScriptRequest\",\n  \"description\": \"ScriptRequest schema from Apache Pig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"script\": {\n      \"type\": \"string\",\n      \"example\": \"A = LOAD 'data.csv';\\nB = FOREACH A GENERATE $0, $1;\"\n    }\n  },\n  \"required\": [\n    \"script\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pig/refs/heads/main/json-schema/apache-pig-script-request-schema.json
tags:
- Big Data
- Data Analysis
- ETL
- Hadoop
- Scripting
- Apache
- Open Source
title: ScriptRequest
---

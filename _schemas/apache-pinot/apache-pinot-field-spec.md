---
description: FieldSpec schema from Apache Pinot
layout: schema
name: FieldSpec
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: dataType
  type: string
- description: ''
  name: notNull
  type: boolean
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-field-spec-schema.json
slug: apache-pinot-field-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-field-spec-schema.json\",\n  \"title\": \"FieldSpec\",\n  \"description\": \"FieldSpec schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"AirlineID\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INT\",\n        \"LONG\",\n        \"FLOAT\",\n        \"DOUBLE\",\n        \"STRING\",\n        \"BYTES\",\n        \"BOOLEAN\",\n        \"TIMESTAMP\",\n        \"JSON\"\n      ],\n      \"example\": \"INT\"\n    },\n    \"notNull\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-field-spec-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: FieldSpec
---

---
description: KeyValue schema from Apache OpenWhisk
layout: schema
name: KeyValue
properties_list:
- description: Parameter key
  name: key
  type: string
- description: Parameter value
  name: value
  type: object
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-key-value-schema.json
slug: apache-openwhisk-key-value
source_filename: apache-openwhisk-key-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-key-value-schema.json\",\n  \"title\": \"KeyValue\",\n  \"description\": \"KeyValue schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter key\",\n      \"example\": \"name\"\n    },\n    \"value\": {\n      \"description\": \"Parameter value\",\n      \"example\": \"World\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-key-value-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: KeyValue
---

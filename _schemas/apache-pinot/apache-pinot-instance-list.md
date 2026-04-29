---
description: InstanceList schema from Apache Pinot
layout: schema
name: InstanceList
properties_list:
- description: ''
  name: instances
  type: array
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-instance-list-schema.json
slug: apache-pinot-instance-list
source_filename: apache-pinot-instance-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-instance-list-schema.json\",\n  \"title\": \"InstanceList\",\n  \"description\": \"InstanceList schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Broker_localhost_8099\",\n        \"Server_localhost_8098\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-instance-list-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: InstanceList
---

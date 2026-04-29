---
description: TableConfig schema from Apache Pinot
layout: schema
name: TableConfig
properties_list:
- description: ''
  name: tableName
  type: string
- description: ''
  name: tableType
  type: string
- description: ''
  name: segmentsConfig
  type: object
- description: ''
  name: tenants
  type: object
provider_name: Apache Pinot
provider_slug: apache-pinot
schema_file: json-schema/apache-pinot-table-config-schema.json
slug: apache-pinot-table-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-table-config-schema.json\",\n  \"title\": \"TableConfig\",\n  \"description\": \"TableConfig schema from Apache Pinot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"example\": \"myTable\"\n    },\n    \"tableType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OFFLINE\",\n        \"REALTIME\"\n      ],\n      \"example\": \"OFFLINE\"\n    },\n    \"segmentsConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"replication\": {\n          \"type\": \"string\",\n          \"example\": \"1\"\n        },\n        \"timeColumnName\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"tenants\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"broker\": {\n       \
  \   \"type\": \"string\",\n          \"example\": \"DefaultTenant\"\n        },\n        \"server\": {\n          \"type\": \"string\",\n          \"example\": \"DefaultTenant\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pinot/refs/heads/main/json-schema/apache-pinot-table-config-schema.json
tags:
- Analytics
- Database
- Low Latency
- OLAP
- Real-Time
- Apache
- Open Source
title: TableConfig
---

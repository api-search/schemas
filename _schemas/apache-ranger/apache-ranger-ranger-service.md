---
description: Ranger service definition
layout: schema
name: RangerService
properties_list:
- description: Service identifier
  name: id
  type: integer
- description: Service name
  name: name
  type: string
- description: Service type (hdfs, hive, hbase, kafka, etc.)
  name: type
  type: string
- description: Service description
  name: description
  type: string
- description: Whether the service is active
  name: isEnabled
  type: boolean
- description: Service connection configuration
  name: configs
  type: object
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-ranger-service-schema.json
slug: apache-ranger-ranger-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-ranger-service-schema.json\",\n  \"title\": \"RangerService\",\n  \"description\": \"Ranger service definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Service identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Service type (hdfs, hive, hbase, kafka, etc.)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Service description\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the service is active\"\n    },\n    \"configs\": {\n      \"type\": \"object\",\n      \"description\": \"Service connection\
  \ configuration\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-ranger-service-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: RangerService
---

---
description: HBase cluster version information
layout: schema
name: ClusterVersion
properties_list:
- description: HBase server version
  name: Server
  type: string
- description: JVM version
  name: JVM
  type: string
- description: Operating system
  name: OS
  type: string
- description: REST API version
  name: REST
  type: string
- description: Jersey framework version
  name: Jersey
  type: string
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-clusterversion-schema.json
slug: hbase-rest-clusterversion
source_filename: hbase-rest-clusterversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-clusterversion-schema.json\",\n  \"title\": \"ClusterVersion\",\n  \"type\": \"object\",\n  \"description\": \"HBase cluster version information\",\n  \"properties\": {\n    \"Server\": {\n      \"type\": \"string\",\n      \"description\": \"HBase server version\",\n      \"example\": \"2.5.7\"\n    },\n    \"JVM\": {\n      \"type\": \"string\",\n      \"description\": \"JVM version\",\n      \"example\": \"Oracle Corporation 11.0.20\"\n    },\n    \"OS\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system\",\n      \"example\": \"Linux 5.15.0\"\n    },\n    \"REST\": {\n      \"type\": \"string\",\n      \"description\": \"REST API version\",\n      \"example\": \"0.0.3\"\n    },\n    \"Jersey\": {\n      \"type\": \"string\",\n      \"description\": \"Jersey framework version\",\n      \"example\": \"1.19\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-clusterversion-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: ClusterVersion
---

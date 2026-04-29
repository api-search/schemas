---
description: Describes the starting parameters for a SQL-based Kinesis Data Analytics application.
layout: schema
name: SqlRunConfiguration
properties_list:
- description: ''
  name: InputId
  type: object
- description: ''
  name: InputStartingPositionConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-sql-run-configuration-schema.json
slug: amazon-managed-apache-flink-sql-run-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-run-configuration-schema.json\",\n  \"title\": \"SqlRunConfiguration\",\n  \"description\": \"Describes the starting parameters for a SQL-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The input source ID. You can get this ID by calling the <a>DescribeApplication</a> operation. \"\n        }\n      ]\n    },\n    \"InputStartingPositionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputStartingPositionConfiguration\"\n        },\n        {\n          \"description\": \"The point at which you want the application to start\
  \ processing records from the streaming source. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputId\",\n    \"InputStartingPositionConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-sql-run-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: SqlRunConfiguration
---

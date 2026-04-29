---
description: StopApplicationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: StopApplicationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: Force
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-stop-application-request-schema.json
slug: amazon-managed-apache-flink-stop-application-request
source_filename: amazon-managed-apache-flink-stop-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-stop-application-request-schema.json\",\n  \"title\": \"StopApplicationRequest\",\n  \"description\": \"StopApplicationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the running application to stop.\"\n        }\n      ]\n    },\n    \"Force\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to force the application to stop. If you set <code>Force</code> to <code>true</code>, Kinesis Data Analytics\
  \ stops the application without taking a snapshot. </p> <note> <p>Force-stopping your application may lead to data loss or duplication. To prevent data loss or duplicate processing of data during application restarts, we recommend you to take frequent snapshots of your application.</p> </note> <p>You can only force stop a Flink-based Kinesis Data Analytics application. You can't force stop a SQL-based Kinesis Data Analytics application.</p> <p>The application must be in the <code>STARTING</code>, <code>UPDATING</code>, <code>STOPPING</code>, <code>AUTOSCALING</code>, or <code>RUNNING</code> status. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-stop-application-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: StopApplicationRequest
---

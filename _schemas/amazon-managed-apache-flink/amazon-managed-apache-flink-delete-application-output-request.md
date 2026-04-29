---
description: DeleteApplicationOutputRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DeleteApplicationOutputRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: OutputId
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-delete-application-output-request-schema.json
slug: amazon-managed-apache-flink-delete-application-output-request
source_filename: amazon-managed-apache-flink-delete-application-output-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-output-request-schema.json\",\n  \"title\": \"DeleteApplicationOutputRequest\",\n  \"description\": \"DeleteApplicationOutputRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The application name.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The application version. You can use the <a>DescribeApplication</a> operation to get the current application\
  \ version. If the version specified is not the current version, the <code>ConcurrentModificationException</code> is returned. \"\n        }\n      ]\n    },\n    \"OutputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the configuration to delete. Each output configuration that is added to the application (either when the application is created or later) using the <a>AddApplicationOutput</a> operation has a unique ID. You need to provide the ID to uniquely identify the output configuration that you want to delete from the application configuration. You can use the <a>DescribeApplication</a> operation to get the specific <code>OutputId</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"CurrentApplicationVersionId\",\n    \"OutputId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-output-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeleteApplicationOutputRequest
---

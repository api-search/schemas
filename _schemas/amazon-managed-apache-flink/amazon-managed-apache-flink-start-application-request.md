---
description: StartApplicationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: StartApplicationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: RunConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-start-application-request-schema.json
slug: amazon-managed-apache-flink-start-application-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-start-application-request-schema.json\",\n  \"title\": \"StartApplicationRequest\",\n  \"description\": \"StartApplicationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application.\"\n        }\n      ]\n    },\n    \"RunConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunConfiguration\"\n        },\n        {\n          \"description\": \"Identifies the run configuration (start parameters) of a Kinesis Data Analytics application.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"ApplicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-start-application-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: StartApplicationRequest
---

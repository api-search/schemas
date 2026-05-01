---
description: DeleteApplicationReferenceDataSourceRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DeleteApplicationReferenceDataSourceRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: ReferenceId
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-delete-application-reference-data-source-request-schema.json
slug: amazon-managed-apache-flink-delete-application-reference-data-source-request
source_filename: amazon-managed-apache-flink-delete-application-reference-data-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-reference-data-source-request-schema.json\",\n  \"title\": \"DeleteApplicationReferenceDataSourceRequest\",\n  \"description\": \"DeleteApplicationReferenceDataSourceRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an existing application.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The current application version. You can use\
  \ the <a>DescribeApplication</a> operation to get the current application version. If the version specified is not the current version, the <code>ConcurrentModificationException</code> is returned.\"\n        }\n      ]\n    },\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the reference data source. When you add a reference data source to your application using the <a>AddApplicationReferenceDataSource</a>, Kinesis Data Analytics assigns an ID. You can use the <a>DescribeApplication</a> operation to get the reference ID. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"CurrentApplicationVersionId\",\n    \"ReferenceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-reference-data-source-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeleteApplicationReferenceDataSourceRequest
---

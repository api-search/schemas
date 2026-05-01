---
description: ListApplicationVersionsRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: ListApplicationVersionsRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-list-application-versions-request-schema.json
slug: amazon-managed-apache-flink-list-application-versions-request
source_filename: amazon-managed-apache-flink-list-application-versions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-application-versions-request-schema.json\",\n  \"title\": \"ListApplicationVersionsRequest\",\n  \"description\": \"ListApplicationVersionsRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application for which you want to list all versions.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListApplicationVersionsInputLimit\"\n        },\n        {\n          \"description\": \"The maximum number of versions to list in this invocation of\
  \ the operation.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a previous invocation of this operation returned a pagination token, pass it into this value to retrieve the next set of results. For more information about pagination, see <a href=\\\"https://docs.aws.amazon.com/cli/latest/userguide/pagination.html\\\">Using the Amazon Command Line Interface's Pagination Options</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-application-versions-request-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ListApplicationVersionsRequest
---

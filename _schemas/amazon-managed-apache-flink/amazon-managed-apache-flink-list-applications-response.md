---
description: ListApplicationsResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: ListApplicationsResponse
properties_list:
- description: ''
  name: ApplicationSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-list-applications-response-schema.json
slug: amazon-managed-apache-flink-list-applications-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-applications-response-schema.json\",\n  \"title\": \"ListApplicationsResponse\",\n  \"description\": \"ListApplicationsResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationSummaries\"\n        },\n        {\n          \"description\": \"A list of <code>ApplicationSummary</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The pagination token for the next set of results, or <code>null</code> if there are no additional results.\
  \ Pass this token into a subsequent command to retrieve the next set of items For more information about pagination, see <a href=\\\"https://docs.aws.amazon.com/cli/latest/userguide/pagination.html\\\">Using the Amazon Command Line Interface's Pagination Options</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-applications-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ListApplicationsResponse
---

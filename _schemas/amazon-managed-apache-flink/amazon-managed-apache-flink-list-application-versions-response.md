---
description: ListApplicationVersionsResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: ListApplicationVersionsResponse
properties_list:
- description: ''
  name: ApplicationVersionSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-list-application-versions-response-schema.json
slug: amazon-managed-apache-flink-list-application-versions-response
source_filename: amazon-managed-apache-flink-list-application-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-application-versions-response-schema.json\",\n  \"title\": \"ListApplicationVersionsResponse\",\n  \"description\": \"ListApplicationVersionsResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationVersionSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionSummaries\"\n        },\n        {\n          \"description\": \"<p>A list of the application versions and the associated configuration summaries. The list includes application versions that were rolled back.</p> <p>To get the complete description of a specific application version, invoke the <a>DescribeApplicationVersion</a> operation.</p>\"\n        }\n      ]\n    },\n    \"\
  NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token for the next set of results, or <code>null</code> if there are no additional results. To retrieve the next set of items, pass this token into a subsequent invocation of this operation. For more information about pagination, see <a href=\\\"https://docs.aws.amazon.com/cli/latest/userguide/pagination.html\\\">Using the Amazon Command Line Interface's Pagination Options</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-list-application-versions-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ListApplicationVersionsResponse
---

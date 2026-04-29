---
description: UpdateApplicationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: UpdateApplicationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: ApplicationConfigurationUpdate
  type: object
- description: ''
  name: ServiceExecutionRoleUpdate
  type: object
- description: ''
  name: RunConfigurationUpdate
  type: object
- description: ''
  name: CloudWatchLoggingOptionUpdates
  type: object
- description: ''
  name: ConditionalToken
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-update-application-request-schema.json
slug: amazon-managed-apache-flink-update-application-request
source_filename: amazon-managed-apache-flink-update-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-update-application-request-schema.json\",\n  \"title\": \"UpdateApplicationRequest\",\n  \"description\": \"UpdateApplicationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application to update.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The current application version ID. You must provide the <code>CurrentApplicationVersionId</code> or\
  \ the <code>ConditionalToken</code>.You can retrieve the application version ID using <a>DescribeApplication</a>. For better concurrency support, use the <code>ConditionalToken</code> parameter instead of <code>CurrentApplicationVersionId</code>.\"\n        }\n      ]\n    },\n    \"ApplicationConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes application configuration updates.\"\n        }\n      ]\n    },\n    \"ServiceExecutionRoleUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"Describes updates to the service execution role.\"\n        }\n      ]\n    },\n    \"RunConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunConfigurationUpdate\"\n        },\n        {\n          \"description\": \"\
  Describes updates to the application's starting parameters.\"\n        }\n      ]\n    },\n    \"CloudWatchLoggingOptionUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLoggingOptionUpdates\"\n        },\n        {\n          \"description\": \"Describes application Amazon CloudWatch logging option updates. You can only update existing CloudWatch logging options with this action. To add a new CloudWatch logging option, use <a>AddApplicationCloudWatchLoggingOption</a>.\"\n        }\n      ]\n    },\n    \"ConditionalToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionalToken\"\n        },\n        {\n          \"description\": \"A value you use to implement strong concurrency for application updates. You must provide the <code>CurrentApplicationVersionId</code> or the <code>ConditionalToken</code>. You get the application's current <code>ConditionalToken</code> using <a>DescribeApplication</a>. For\
  \ better concurrency support, use the <code>ConditionalToken</code> parameter instead of <code>CurrentApplicationVersionId</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-update-application-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: UpdateApplicationRequest
---

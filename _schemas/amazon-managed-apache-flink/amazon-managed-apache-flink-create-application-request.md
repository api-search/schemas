---
description: CreateApplicationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: CreateApplicationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: ApplicationDescription
  type: object
- description: ''
  name: RuntimeEnvironment
  type: object
- description: ''
  name: ServiceExecutionRole
  type: object
- description: ''
  name: ApplicationConfiguration
  type: object
- description: ''
  name: CloudWatchLoggingOptions
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ApplicationMode
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-create-application-request-schema.json
slug: amazon-managed-apache-flink-create-application-request
source_filename: amazon-managed-apache-flink-create-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-create-application-request-schema.json\",\n  \"title\": \"CreateApplicationRequest\",\n  \"description\": \"CreateApplicationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of your application (for example, <code>sample-app</code>).\"\n        }\n      ]\n    },\n    \"ApplicationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationDescription\"\n        },\n        {\n          \"description\": \"A summary description of the application.\"\n        }\n      ]\n    },\n\
  \    \"RuntimeEnvironment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeEnvironment\"\n        },\n        {\n          \"description\": \"The runtime environment for the application.\"\n        }\n      ]\n    },\n    \"ServiceExecutionRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"The IAM role used by the application to access Kinesis data streams, Kinesis Data Firehose delivery streams, Amazon S3 objects, and other external resources.\"\n        }\n      ]\n    },\n    \"ApplicationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationConfiguration\"\n        },\n        {\n          \"description\": \"Use this parameter to configure the application.\"\n        }\n      ]\n    },\n    \"CloudWatchLoggingOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLoggingOptions\"\
  \n        },\n        {\n          \"description\": \"Use this parameter to configure an Amazon CloudWatch log stream to monitor application configuration errors. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A list of one or more tags to assign to the application. A tag is a key-value pair that identifies an application. Note that the maximum number of application tags includes system tags. The maximum number of user-defined application tags is 50. For more information, see <a href=\\\"https://docs.aws.amazon.com/kinesisanalytics/latest/java/how-tagging.html\\\">Using Tagging</a>.\"\n        }\n      ]\n    },\n    \"ApplicationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMode\"\n        },\n        {\n          \"description\": \"Use the <code>STREAMING</code> mode to create a Kinesis Data Analytics\
  \ For Flink application. To create a Kinesis Data Analytics Studio notebook, use the <code>INTERACTIVE</code> mode.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"RuntimeEnvironment\",\n    \"ServiceExecutionRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-create-application-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CreateApplicationRequest
---

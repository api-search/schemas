---
description: Describes configuration parameters for a Flink-based Kinesis Data Analytics application.
layout: schema
name: FlinkApplicationConfigurationDescription
properties_list:
- description: ''
  name: CheckpointConfigurationDescription
  type: object
- description: ''
  name: MonitoringConfigurationDescription
  type: object
- description: ''
  name: ParallelismConfigurationDescription
  type: object
- description: ''
  name: JobPlanDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-flink-application-configuration-description-schema.json
slug: amazon-managed-apache-flink-flink-application-configuration-description
source_filename: amazon-managed-apache-flink-flink-application-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-application-configuration-description-schema.json\",\n  \"title\": \"FlinkApplicationConfigurationDescription\",\n  \"description\": \"Describes configuration parameters for a Flink-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CheckpointConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckpointConfigurationDescription\"\n        },\n        {\n          \"description\": \"Describes an application's checkpointing configuration. Checkpointing is the process of persisting application state for fault tolerance.\"\n        }\n      ]\n    },\n    \"MonitoringConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MonitoringConfigurationDescription\"\
  \n        },\n        {\n          \"description\": \"Describes configuration parameters for Amazon CloudWatch logging for an application.\"\n        }\n      ]\n    },\n    \"ParallelismConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParallelismConfigurationDescription\"\n        },\n        {\n          \"description\": \"Describes parameters for how an application executes multiple tasks simultaneously.\"\n        }\n      ]\n    },\n    \"JobPlanDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobPlanDescription\"\n        },\n        {\n          \"description\": \"The job plan for an application. For more information about the job plan, see <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/internals/job_scheduling.html\\\">Jobs and Scheduling</a> in the <a href=\\\"https://ci.apache.org/projects/flink/flink-docs-release-1.8/\\\">Apache Flink Documentation</a>.\
  \ To retrieve the job plan for the application, use the <a>DescribeApplicationRequest$IncludeAdditionalDetails</a> parameter of the <a>DescribeApplication</a> operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-flink-application-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: FlinkApplicationConfigurationDescription
---

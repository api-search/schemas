---
description: Describes updates to parameters for how an application executes multiple tasks simultaneously.
layout: schema
name: ParallelismConfigurationUpdate
properties_list:
- description: ''
  name: ConfigurationTypeUpdate
  type: object
- description: ''
  name: ParallelismUpdate
  type: object
- description: ''
  name: ParallelismPerKPUUpdate
  type: object
- description: ''
  name: AutoScalingEnabledUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-parallelism-configuration-update-schema.json
slug: amazon-managed-apache-flink-parallelism-configuration-update
source_filename: amazon-managed-apache-flink-parallelism-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-parallelism-configuration-update-schema.json\",\n  \"title\": \"ParallelismConfigurationUpdate\",\n  \"description\": \"Describes updates to parameters for how an application executes multiple tasks simultaneously.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationTypeUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"description\": \"Describes updates to whether the application uses the default parallelism for the Kinesis Data Analytics service, or if a custom parallelism is used. You must set this property to <code>CUSTOM</code> in order to change your application's <code>AutoScalingEnabled</code>, <code>Parallelism</code>, or <code>ParallelismPerKPU</code>\
  \ properties.\"\n        }\n      ]\n    },\n    \"ParallelismUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Parallelism\"\n        },\n        {\n          \"description\": \"Describes updates to the initial number of parallel tasks an application can perform. If <code>AutoScalingEnabled</code> is set to True, then Kinesis Data Analytics can increase the <code>CurrentParallelism</code> value in response to application load. The service can increase <code>CurrentParallelism</code> up to the maximum parallelism, which is <code>ParalellismPerKPU</code> times the maximum KPUs for the application. The maximum KPUs for an application is 32 by default, and can be increased by requesting a limit increase. If application load is reduced, the service will reduce <code>CurrentParallelism</code> down to the <code>Parallelism</code> setting.\"\n        }\n      ]\n    },\n    \"ParallelismPerKPUUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/ParallelismPerKPU\"\n        },\n        {\n          \"description\": \"Describes updates to the number of parallel tasks an application can perform per Kinesis Processing Unit (KPU) used by the application.\"\n        }\n      ]\n    },\n    \"AutoScalingEnabledUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Describes updates to whether the Kinesis Data Analytics service can increase the parallelism of a Flink-based Kinesis Data Analytics application in response to increased throughput.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-parallelism-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ParallelismConfigurationUpdate
---

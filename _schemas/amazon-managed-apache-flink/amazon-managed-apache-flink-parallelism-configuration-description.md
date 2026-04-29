---
description: Describes parameters for how a Flink-based Kinesis Data Analytics application executes multiple tasks simultaneously.
layout: schema
name: ParallelismConfigurationDescription
properties_list:
- description: ''
  name: ConfigurationType
  type: object
- description: ''
  name: Parallelism
  type: object
- description: ''
  name: ParallelismPerKPU
  type: object
- description: ''
  name: CurrentParallelism
  type: object
- description: ''
  name: AutoScalingEnabled
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-parallelism-configuration-description-schema.json
slug: amazon-managed-apache-flink-parallelism-configuration-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-parallelism-configuration-description-schema.json\",\n  \"title\": \"ParallelismConfigurationDescription\",\n  \"description\": \"Describes parameters for how a Flink-based Kinesis Data Analytics application executes multiple tasks simultaneously.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"description\": \"Describes whether the application uses the default parallelism for the Kinesis Data Analytics service. \"\n        }\n      ]\n    },\n    \"Parallelism\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Parallelism\"\n        },\n        {\n          \"description\":\
  \ \"Describes the initial number of parallel tasks that a Flink-based Kinesis Data Analytics application can perform. If <code>AutoScalingEnabled</code> is set to True, then Kinesis Data Analytics can increase the <code>CurrentParallelism</code> value in response to application load. The service can increase <code>CurrentParallelism</code> up to the maximum parallelism, which is <code>ParalellismPerKPU</code> times the maximum KPUs for the application. The maximum KPUs for an application is 32 by default, and can be increased by requesting a limit increase. If application load is reduced, the service can reduce the <code>CurrentParallelism</code> value down to the <code>Parallelism</code> setting.\"\n        }\n      ]\n    },\n    \"ParallelismPerKPU\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParallelismPerKPU\"\n        },\n        {\n          \"description\": \"Describes the number of parallel tasks that a Flink-based Kinesis Data Analytics application\
  \ can perform per Kinesis Processing Unit (KPU) used by the application.\"\n        }\n      ]\n    },\n    \"CurrentParallelism\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Parallelism\"\n        },\n        {\n          \"description\": \"Describes the current number of parallel tasks that a Flink-based Kinesis Data Analytics application can perform. If <code>AutoScalingEnabled</code> is set to True, Kinesis Data Analytics can increase this value in response to application load. The service can increase this value up to the maximum parallelism, which is <code>ParalellismPerKPU</code> times the maximum KPUs for the application. The maximum KPUs for an application is 32 by default, and can be increased by requesting a limit increase. If application load is reduced, the service can reduce the <code>CurrentParallelism</code> value down to the <code>Parallelism</code> setting.\"\n        }\n      ]\n    },\n    \"AutoScalingEnabled\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Describes whether the Kinesis Data Analytics service can increase the parallelism of the application in response to increased throughput.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-parallelism-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ParallelismConfigurationDescription
---

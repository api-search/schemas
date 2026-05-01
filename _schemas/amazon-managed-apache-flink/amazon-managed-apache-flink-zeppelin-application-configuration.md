---
description: The configuration of a Kinesis Data Analytics Studio notebook.
layout: schema
name: ZeppelinApplicationConfiguration
properties_list:
- description: ''
  name: MonitoringConfiguration
  type: object
- description: ''
  name: CatalogConfiguration
  type: object
- description: ''
  name: DeployAsApplicationConfiguration
  type: object
- description: ''
  name: CustomArtifactsConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-schema.json
slug: amazon-managed-apache-flink-zeppelin-application-configuration
source_filename: amazon-managed-apache-flink-zeppelin-application-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-schema.json\",\n  \"title\": \"ZeppelinApplicationConfiguration\",\n  \"description\": \"The configuration of a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MonitoringConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeppelinMonitoringConfiguration\"\n        },\n        {\n          \"description\": \"The monitoring configuration of a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    },\n    \"CatalogConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogConfiguration\"\n        },\n        {\n          \"description\": \"The Amazon Glue Data Catalog that you use in queries\
  \ in a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    },\n    \"DeployAsApplicationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeployAsApplicationConfiguration\"\n        },\n        {\n          \"description\": \"The information required to deploy a Kinesis Data Analytics Studio notebook as an application with durable state.\"\n        }\n      ]\n    },\n    \"CustomArtifactsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomArtifactsConfigurationList\"\n        },\n        {\n          \"description\": \"Custom artifacts are dependency JARs and user-defined functions (UDF).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ZeppelinApplicationConfiguration
---

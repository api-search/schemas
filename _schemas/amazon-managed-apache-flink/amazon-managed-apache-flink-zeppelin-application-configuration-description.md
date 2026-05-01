---
description: The configuration of a Kinesis Data Analytics Studio notebook.
layout: schema
name: ZeppelinApplicationConfigurationDescription
properties_list:
- description: ''
  name: MonitoringConfigurationDescription
  type: object
- description: ''
  name: CatalogConfigurationDescription
  type: object
- description: ''
  name: DeployAsApplicationConfigurationDescription
  type: object
- description: ''
  name: CustomArtifactsConfigurationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-description-schema.json
slug: amazon-managed-apache-flink-zeppelin-application-configuration-description
source_filename: amazon-managed-apache-flink-zeppelin-application-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-description-schema.json\",\n  \"title\": \"ZeppelinApplicationConfigurationDescription\",\n  \"description\": \"The configuration of a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MonitoringConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeppelinMonitoringConfigurationDescription\"\n        },\n        {\n          \"description\": \"The monitoring configuration of a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    },\n    \"CatalogConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogConfigurationDescription\"\n        },\n        {\n          \"\
  description\": \"The Amazon Glue Data Catalog that is associated with the Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    },\n    \"DeployAsApplicationConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeployAsApplicationConfigurationDescription\"\n        },\n        {\n          \"description\": \"The parameters required to deploy a Kinesis Data Analytics Studio notebook as an application with durable state.\"\n        }\n      ]\n    },\n    \"CustomArtifactsConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomArtifactsConfigurationDescriptionList\"\n        },\n        {\n          \"description\": \"Custom artifacts are dependency JARs and user-defined functions (UDF).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MonitoringConfigurationDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ZeppelinApplicationConfigurationDescription
---

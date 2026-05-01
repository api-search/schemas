---
description: Updates to the configuration of Kinesis Data Analytics Studio notebook.
layout: schema
name: ZeppelinApplicationConfigurationUpdate
properties_list:
- description: ''
  name: MonitoringConfigurationUpdate
  type: object
- description: ''
  name: CatalogConfigurationUpdate
  type: object
- description: ''
  name: DeployAsApplicationConfigurationUpdate
  type: object
- description: ''
  name: CustomArtifactsConfigurationUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-update-schema.json
slug: amazon-managed-apache-flink-zeppelin-application-configuration-update
source_filename: amazon-managed-apache-flink-zeppelin-application-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-update-schema.json\",\n  \"title\": \"ZeppelinApplicationConfigurationUpdate\",\n  \"description\": \"Updates to the configuration of Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MonitoringConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeppelinMonitoringConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Updates to the monitoring configuration of a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    },\n    \"CatalogConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogConfigurationUpdate\"\n        },\n        {\n          \"description\"\
  : \"Updates to the configuration of the Amazon Glue Data Catalog that is associated with the Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    },\n    \"DeployAsApplicationConfigurationUpdate\": {\n      \"$ref\": \"#/components/schemas/DeployAsApplicationConfigurationUpdate\"\n    },\n    \"CustomArtifactsConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomArtifactsConfigurationList\"\n        },\n        {\n          \"description\": \"Updates to the customer artifacts. Custom artifacts are dependency JAR files and user-defined functions (UDF).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-application-configuration-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ZeppelinApplicationConfigurationUpdate
---

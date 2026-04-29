---
description: The configuration information required to deploy an Amazon Data Analytics Studio notebook as an application with durable state.
layout: schema
name: DeployAsApplicationConfigurationDescription
properties_list:
- description: ''
  name: S3ContentLocationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-deploy-as-application-configuration-description-schema.json
slug: amazon-managed-apache-flink-deploy-as-application-configuration-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-deploy-as-application-configuration-description-schema.json\",\n  \"title\": \"DeployAsApplicationConfigurationDescription\",\n  \"description\": \"The configuration information required to deploy an Amazon Data Analytics Studio notebook as an application with durable state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3ContentLocationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ContentBaseLocationDescription\"\n        },\n        {\n          \"description\": \"The location that holds the data required to specify an Amazon Data Analytics application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3ContentLocationDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-deploy-as-application-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeployAsApplicationConfigurationDescription
---

---
description: The information required to deploy a Kinesis Data Analytics Studio notebook as an application with durable state.
layout: schema
name: DeployAsApplicationConfiguration
properties_list:
- description: ''
  name: S3ContentLocation
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-deploy-as-application-configuration-schema.json
slug: amazon-managed-apache-flink-deploy-as-application-configuration
source_filename: amazon-managed-apache-flink-deploy-as-application-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-deploy-as-application-configuration-schema.json\",\n  \"title\": \"DeployAsApplicationConfiguration\",\n  \"description\": \"The information required to deploy a Kinesis Data Analytics Studio notebook as an application with durable state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3ContentLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ContentBaseLocation\"\n        },\n        {\n          \"description\": \"The description of an Amazon S3 object that contains the Amazon Data Analytics application, including the Amazon Resource Name (ARN) of the S3 bucket, the name of the Amazon S3 object that contains the data, and the version number of the Amazon S3 object that contains the data. \"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"S3ContentLocation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-deploy-as-application-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeployAsApplicationConfiguration
---

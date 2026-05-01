---
description: Describes the parameters of a VPC used by the application.
layout: schema
name: VpcConfiguration
properties_list:
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-vpc-configuration-schema.json
slug: amazon-managed-apache-flink-vpc-configuration
source_filename: amazon-managed-apache-flink-vpc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-vpc-configuration-schema.json\",\n  \"title\": \"VpcConfiguration\",\n  \"description\": \"Describes the parameters of a VPC used by the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"The array of <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_Subnet.html\\\">Subnet</a> IDs used by the VPC configuration.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The array of <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_SecurityGroup.html\\\
  \">SecurityGroup</a> IDs used by the VPC configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetIds\",\n    \"SecurityGroupIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-vpc-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: VpcConfiguration
---

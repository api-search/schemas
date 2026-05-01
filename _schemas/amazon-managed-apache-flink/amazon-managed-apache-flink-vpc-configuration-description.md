---
description: Describes the parameters of a VPC used by the application.
layout: schema
name: VpcConfigurationDescription
properties_list:
- description: ''
  name: VpcConfigurationId
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-vpc-configuration-description-schema.json
slug: amazon-managed-apache-flink-vpc-configuration-description
source_filename: amazon-managed-apache-flink-vpc-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-vpc-configuration-description-schema.json\",\n  \"title\": \"VpcConfigurationDescription\",\n  \"description\": \"Describes the parameters of a VPC used by the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the VPC configuration.\"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The ID of the associated VPC.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n\
  \        },\n        {\n          \"description\": \"The array of <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_Subnet.html\\\">Subnet</a> IDs used by the VPC configuration.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"The array of <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_SecurityGroup.html\\\">SecurityGroup</a> IDs used by the VPC configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcConfigurationId\",\n    \"VpcId\",\n    \"SubnetIds\",\n    \"SecurityGroupIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-vpc-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: VpcConfigurationDescription
---

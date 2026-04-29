---
description: Describes updates to the VPC configuration used by the application.
layout: schema
name: VpcConfigurationUpdate
properties_list:
- description: ''
  name: VpcConfigurationId
  type: object
- description: ''
  name: SubnetIdUpdates
  type: object
- description: ''
  name: SecurityGroupIdUpdates
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-vpc-configuration-update-schema.json
slug: amazon-managed-apache-flink-vpc-configuration-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-vpc-configuration-update-schema.json\",\n  \"title\": \"VpcConfigurationUpdate\",\n  \"description\": \"Describes updates to the VPC configuration used by the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"Describes an update to the ID of the VPC configuration.\"\n        }\n      ]\n    },\n    \"SubnetIdUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"Describes updates to the array of <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_Subnet.html\\\">Subnet</a> IDs\
  \ used by the VPC configuration.\"\n        }\n      ]\n    },\n    \"SecurityGroupIdUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIds\"\n        },\n        {\n          \"description\": \"Describes updates to the array of <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_SecurityGroup.html\\\">SecurityGroup</a> IDs used by the VPC configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcConfigurationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-vpc-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: VpcConfigurationUpdate
---

---
description: The proposed virtual private cloud (VPC) configuration for the Amazon S3 access point. VPC configuration does not apply to multi-region access points. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_VpcConfiguration.html">VpcConfiguration</a>.
layout: schema
name: VpcConfiguration
properties_list:
- description: ''
  name: vpcId
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-vpc-configuration-schema.json
slug: iam-access-analyzer-vpc-configuration
source_filename: iam-access-analyzer-vpc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-vpc-configuration-schema.json\",\n  \"title\": \"VpcConfiguration\",\n  \"description\": \"The proposed virtual private cloud (VPC) configuration for the Amazon S3 access point. VPC configuration does not apply to multi-region access points. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_VpcConfiguration.html\\\">VpcConfiguration</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \" If this field is specified, this access point will only allow connections from the specified VPC ID. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vpcId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-vpc-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: VpcConfiguration
---

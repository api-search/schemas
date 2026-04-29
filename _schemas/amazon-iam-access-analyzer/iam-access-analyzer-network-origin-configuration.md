---
description: The proposed <code>InternetConfiguration</code> or <code>VpcConfiguration</code> to apply to the Amazon S3 access point. <code>VpcConfiguration</code> does not apply to multi-region access points. You can make the access point accessible from the internet, or you can specify that all requests made through that access point must originate from a specific virtual private cloud (VPC). You can specify only one type of network configuration. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/creating-access-points.html">Creating access points</a>.
layout: schema
name: NetworkOriginConfiguration
properties_list:
- description: The proposed virtual private cloud (VPC) configuration for the Amazon S3 access point. VPC configuration does not apply to multi-region access points. For more information, see <a href="https://docs.a
  name: vpcConfiguration
  type: object
- description: ''
  name: internetConfiguration
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-network-origin-configuration-schema.json
slug: iam-access-analyzer-network-origin-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-network-origin-configuration-schema.json\",\n  \"title\": \"NetworkOriginConfiguration\",\n  \"description\": \"The proposed <code>InternetConfiguration</code> or <code>VpcConfiguration</code> to apply to the Amazon S3 access point. <code>VpcConfiguration</code> does not apply to multi-region access points. You can make the access point accessible from the internet, or you can specify that all requests made through that access point must originate from a specific virtual private cloud (VPC). You can specify only one type of network configuration. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/creating-access-points.html\\\">Creating access points</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vpcConfiguration\": {\n   \
  \   \"type\": \"object\",\n      \"required\": [\n        \"vpcId\"\n      ],\n      \"properties\": {\n        \"vpcId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/VpcId\"\n            },\n            {\n              \"description\": \" If this field is specified, this access point will only allow connections from the specified VPC ID. \"\n            }\n          ]\n        }\n      },\n      \"description\": \"The proposed virtual private cloud (VPC) configuration for the Amazon S3 access point. VPC configuration does not apply to multi-region access points. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_VpcConfiguration.html\\\">VpcConfiguration</a>. \"\n    },\n    \"internetConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InternetConfiguration\"\n        },\n        {\n          \"description\": \"The configuration for the Amazon S3 access\
  \ point or multi-region access point with an <code>Internet</code> origin.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-network-origin-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: NetworkOriginConfiguration
---

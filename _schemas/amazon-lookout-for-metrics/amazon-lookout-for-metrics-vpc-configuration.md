---
description: Contains configuration information about the Amazon Virtual Private Cloud (VPC).
layout: schema
name: VpcConfiguration
properties_list:
- description: ''
  name: SubnetIdList
  type: object
- description: ''
  name: SecurityGroupIdList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-vpc-configuration-schema.json
slug: amazon-lookout-for-metrics-vpc-configuration
source_filename: amazon-lookout-for-metrics-vpc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-vpc-configuration-schema.json\",\n  \"title\": \"VpcConfiguration\",\n  \"description\": \"Contains configuration information about the Amazon Virtual Private Cloud (VPC).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIdList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIdList\"\n        },\n        {\n          \"description\": \"An array of strings containing the Amazon VPC subnet IDs (e.g., <code>subnet-0bb1c79de3EXAMPLE</code>.\"\n        }\n      ]\n    },\n    \"SecurityGroupIdList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIdList\"\n        },\n        {\n          \"description\": \"An array of strings containing the list of security groups.\"\n       \
  \ }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetIdList\",\n    \"SecurityGroupIdList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-vpc-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: VpcConfiguration
---
